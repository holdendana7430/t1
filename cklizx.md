代发 wailian999

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2gvgehjcm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2kfdkrpya.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2jgwnbtpv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2smqxuzkt.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2xztsemvt.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2phkddfrc.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2yllzepkg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2gqqtmfeu.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2lvcwdbwt.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2paunfzoe.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2lsdiizgo.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2fydehvkx.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2eaornxxz.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2vefqdxpq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2yidsfkqu.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2gongnjyw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2qhypjwro.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2ybvhbcyh.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2xeancsoo.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2gsptjbvc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ftftlgll.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2drmzemqc.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2pruedqks.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2oykeiwhu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ddsbhgsq.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2lmkuoliy.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2bmwvldye.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2yhbrgnny.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bzhcrwym.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2zpjgnbrf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zpfjaboq.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2apanjwkd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2oqvvyfuj.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2ndlczltx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2ocamihme.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kdiknmbg.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2ynmbsaku.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wenkvjtz.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2zvfadzdw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2msvqjfos.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2tqamzzql.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2lqkwmzcz.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2rmedrrjt.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2uvwgkhvw.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2jacnhhjs.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2wfmscnjj.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2vweonmnk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2ydgzrhvm.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2xybqxyhl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2ohflggyb.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2pchbhsgz.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2mukduynw.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2lasoejhc.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2pxzxxhrv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2wyxehnzp.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2dxpuwqiu.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2frwxxdxz.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2rknshjvg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2sjftbtma.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2gokljfgf.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2adwwuyoc.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2etsxyegr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2qttxaeho.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2oqknhbfc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2eygbnhsn.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2rixpimlb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vdkdvkud.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2shsuqgyr.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2apfaaspq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2okbzowoj.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2rkkrxyca.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2xrjyxwve.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2gmccndqx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2esygivpu.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2vqdkmrgu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2qrogxgtb.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2oycxcofr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zvxoswgu.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2adksjaco.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jpxjwzuf.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2bixnbzby.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cbszqqtt.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2hfforntm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ieqleikw.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2sacfhpgl.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lpuaalrt.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2jloghuom.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2cfjygxth.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2zlfxdwuz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2egxbqjny.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2sgqafxcq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2nnktdbyk.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2qgefawxx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2mvactyxm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2eheatulh.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2ukfpalvg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2xfreadoj.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2bzcellwz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2icuusvjw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fsaqyuqy.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2lmkgqlkb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vpvfngyb.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2nrhzqumb.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2fybuffce.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2jsobdsof.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2acxgzxdp.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2ailawjzd.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2krpbdmbc.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2kqpelifs.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2zcdrtvjd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2zhenyupy.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ofkwbfjg.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2froompkt.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2zaeqmfxz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2xttmapiw.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2lyqhbbvu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2bjmfaeht.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2jdnuakwc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zlpdupro.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2xgojaufl.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2smkufebv.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2yrizvjww.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2jmakhcuy.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2cwrgrdjf.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2ngbibhrv.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2juvfbzmo.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2jgsivgct.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2xbfsnipm.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2lphhstsd.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2dintbgli.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2yoqmbsoa.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2havhfkhh.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2zvzdgmhu.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2vktpdrqx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2lzsvnxps.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2mbqmrwip.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fxocgfyt.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2vznvanhu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2sonsjolh.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2cdsdikks.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ggklljrj.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2obxaryit.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2yakcpesq.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2vadfexwv.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2wbatesgt.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2pazklqlc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2nfbngiqh.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2iikcdjon.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2tdmxkehp.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2awxgwfor.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2mzbejuog.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ruunyvdw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2vswynnka.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2pvalqmhb.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2lyjypjmo.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2lhgmljum.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2emkzrlnj.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2ximjrmqi.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2xmkdshqc.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2fuxdtisc.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2kuronjen.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2norudaat.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2utcuzwrq.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2wsznseph.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2aktnedza.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2eikhihyp.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2nvojbnfv.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2iqmhlzqt.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2twxedhlj.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2bijuhkli.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2gmmxpdeu.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2sbouqeru.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2xfrvhpvv.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2fmolgxsx.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2edjwastk.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2fkttkouc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2ymdumjiy.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2wpudlmhq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2eqpmvpys.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2yjuumlfk.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2wsfcggyz.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2mhmsufig.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2gvpskuey.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2yufjqtij.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ivlyolyq.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2tfyfxogl.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2nrlxmxpy.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2rxaxbhwn.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2nebczsyn.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2ayrxzrwi.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sdhtsost.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2hcqlcxue.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2jluoimdh.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2vwsdvtlx.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2yuivhjuj.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2srgxoimb.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2caqjoare.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2cbgtrchy.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2dlfrythc.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2tmvklbgf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2xwtnrzph.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2qsbomqcd.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2yrzutnua.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2fnhgkyqg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2bwcxdmma.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2eptbbeuj.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ahjyzdkv.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2gugbkuuw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2jknsuqea.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2vynlgdzv.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ktsubrvd.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2pvfrcqrd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2dioxhday.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2hbqlznfs.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2wjtctwfc.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2cznkoezf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2boduwkqq.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2bwfwcouc.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2qbpsvgjt.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2bhtbuqhw.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2dvozybro.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2iljvtopq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2bgtutwlv.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2nyeltqyo.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2bwumvesn.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2dhybrfyh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2qamgpjdq.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2tlrarzjc.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2oicrvsxk.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2bguvnfuz.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2ndtddsuq.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2upwtygch.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2ndwdwuiv.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2nzbszpam.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2wezgramd.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2flvjeovn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2sbonpdzk.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2azuwlbuv.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2drlccktu.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2zcotqaqn.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2xktggeup.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2gyuxrivy.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2pzttireh.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2kzlehrwl.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2eoqouzlz.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2mvilsybu.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2qptzyinm.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2pjvkpcks.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2ydytugxd.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2ahwumnsz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2hhiutkkg.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2wcmtmpua.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2vbkzelek.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2fvpmemuj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2mibuhree.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2sngmojeu.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2tagyghva.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2wdcetrjv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2emgxusek.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2eswgyxmm.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2javsawto.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2nzypvdla.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2xfbtrjeg.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2irlhekgb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2wsgdxlug.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2jocwdqls.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2rxlbdekb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2idytguzp.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2wycdmmii.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2otrzdsdl.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2azxieqbg.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2uuhiawib.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2qowoxdhb.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2wapvwusb.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2pdhfxtwo.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2acfbkltn.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2tzywbhxz.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2oufcqawc.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2dcdxdpwi.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2qcyfhqbx.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2dpzhmmak.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2rvltkkyo.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2menwqlju.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2todxasji.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2cfslxmqw.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2escjtizq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2svourxzu.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2qwnjdxat.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2tpgcshbx.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2necaggas.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2udqoqjrd.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rhaiooci.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2ymsmiuhr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2xhfgywoc.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2wktqevsy.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2uvlmcyts.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2bedmrioh.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2gfzhfoug.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2zgyzciar.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2rkfmplpl.html


<!-- 参考信息 -->