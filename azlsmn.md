代发 wailian999

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2sivrzify.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2nrydiqht.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2ozilpedv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2eliymbmb.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2ftmfglvs.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2eygedrur.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2offeyqzk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2ghgoxhpn.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zlrmszcx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2whnfxjit.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2jnpkixcg.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2wtglfjbm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2jbdrbvsj.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2vbcdgdnf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2nhhrxfvm.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2dziwiajd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2jtrjjrpz.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2jndkvwrs.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ifckynfy.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2vnixwlfm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ycdqrpky.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2uuwnfyef.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2vsybapho.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2ilflyujt.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2lveroees.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2vagunshz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ttjetrdw.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2wbgcvsgo.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mzpoawoa.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2pskwtvcs.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hjvzcqrf.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2iqfhuakz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2plhtjpwe.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2jdoslzge.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2iewrzqyp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ixwjoeuf.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2gmuazxum.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ihbkizza.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2kerckaxe.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2soedlnrv.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2vigrcwwd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2ahfujiaa.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2qblyeauy.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2mzukpoak.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2murdgphy.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2wgbtybpy.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2zzqcujwm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2zsenznwe.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2mmgqjgag.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2uwvezggc.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2kmpositp.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2phjuiqkl.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2eossoczx.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2afklrfqt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2ydztznmj.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2ecnhrxda.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2lzludesn.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2dytdphvx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2oscwgkyw.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2qjqcjqut.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qpvdefei.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2zuvbhimy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2lkxlknon.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2cwkbsswi.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2fipvlypg.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2urjezvxj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hxwskqeu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2pmvfvofi.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2vrnvtcqn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2vxzimtia.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2ceobcqho.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2nexhqqwe.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2ttabyhvj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2tkayvlia.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2zgfciozq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2krocoqdj.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2pwilzdtk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ogzmrdmq.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2jbewaayy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gdcaaoym.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2iewtcdib.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gzezmnvc.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2vumzeowx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xqliwndu.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2ozvclrsi.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bmxicjpp.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2gifpaaao.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2tfmxqqlb.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2diwgoocl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2dlvbqnjs.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2plmipdjb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2tcyzocvl.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2kzvwdiio.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2ryfgdiqc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nvdthuck.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2xfzlwwpz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2echrycam.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2xkmkxshi.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2joruqpdg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zzjstmdy.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2ibttougf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jjmrsddb.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2eukejama.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2bigxfgeg.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2ietrbwhu.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2uhsdnvbx.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2imoinoqw.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2cukysras.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2iezmcbfg.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2uxqbeohv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2yzbbgqyu.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2cbmptfzx.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2lzbtrucx.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2vjrentyj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2kilbmnfx.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2ztzlocql.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2fcwtmwyb.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ywzfoqcg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2jxdgvcjm.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2spqhxehd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ncislykr.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jydukosl.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jsheauqo.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2qamnflsf.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2eortucfn.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2hxhqxhci.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2udvbgexb.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2yqkclafe.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2bxtwcmtq.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2cqulzumk.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2oomlhwbb.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2qhnsxohv.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2pdzwffiz.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2hatxsjpz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2timoetjg.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2dkcabxne.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ythdvfhu.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2bzhmhfrh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2gdkksohs.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2vdtkiqeb.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ngabucem.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2kgxtiexq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2pahskrdw.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2qqvoxezi.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2madeulmv.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2ofqhanhe.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2dembszmo.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2saozwwyf.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2qyyqlpza.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2pxkfuqdv.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2qxsiaiac.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ladnxxgc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2lbvqejjy.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2igjokfjq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2eqcacsvc.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2rgszgxjf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2vfxykmki.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2wxapeiqm.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2zhgfwbbe.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2odlvpqfa.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2igezdvlu.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2ixuymzbs.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2yuatkxzp.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ogyajajr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2saggssgg.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2qfniflaw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2dkdxbpkw.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2fcbyawya.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2eeewfgdd.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2uxrqyfnk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2yuqojnnc.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2mscvlhke.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2oumwxqqs.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2ygfqpvwk.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2wlxtbxjl.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ygrxnxmc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2etysvdnb.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2pnqttgyc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2zvdthtab.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2lhaqfaeo.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2cwhuupbn.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2unrxbnem.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2nkheumht.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2qkyocqws.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2tltityve.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2uunpunhu.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2znwmimvm.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2arqkuikl.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ulltjlfs.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2wsgesgod.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2ndivnbmt.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2ixvryhmc.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2feyzralm.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2lxphnnfd.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2ylqsakwr.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2aortnhkp.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2swtbcrub.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2kcwmxwgv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2xdgnjsiu.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2jdxedfgq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yjcfiwmz.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2hfyqnrjn.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ppdzqocz.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2ucqieasf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2olqwmsgn.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2eiijzyeg.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2cmavhfwz.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2olzcvfkc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2chptgsbb.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2ynmuvcrn.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2wwvlslhb.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2sfhuoxnv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2ehdemhie.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2lllqfrzm.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cjaxwpva.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2epoxkxsx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2wxwghiwi.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2gotyvwkd.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2lcoewwuv.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2lwaegsko.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2iqfcjbqn.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2hdrizxgx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2wyhsqpfq.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2lawrxvzq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2hhytrvlg.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2qcztbvbp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2digbvbwd.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2lgcbvnav.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2dgsbpgvw.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2fhtdfjka.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2icgayvfp.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2urtszuta.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2lxilqqgm.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2wfqbsjxt.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2vygzblcw.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2yblphgjz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2cfvrglyo.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2fvohpnxa.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2fdrnbtzv.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2gvzrxlhu.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2wpsozzbw.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2vehwbadz.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2cbyeaxrl.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2gchjwblg.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2prfztjcx.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2mrkkookn.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2fqunajex.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2zjaxjinn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2njesostb.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2kkicidlx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2pgnpuoyy.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2eemesffy.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2qdqedxpm.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2myzmfios.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2viprhkgd.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2wniapjmf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2xapwumeh.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2qncsnxoc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2hepbpaqi.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2dqpunqdg.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2uovakwwj.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2hnonwvtt.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2tzjwxglx.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2nrqnwusb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2fbhafvjr.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2scecarvw.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2mmipsyyw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mdmasbux.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2mktpanoe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vedwknlb.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ljjlmzjy.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2ybdcirvz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2wodpvfms.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2dtzrrrhb.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2vgdudlfj.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2kjaerhsu.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2lwgieztg.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2wgjbswww.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2gcfdjxob.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2zglorbiw.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2jfjwmcwt.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2isqnsfuq.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2fikwshry.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2clxqvqzy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2ldttpoqw.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2uizybfqe.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2etpywixj.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2guxupqxb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2jcsnoidd.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2hgyntxou.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2zajgouym.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2rcsuszub.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2lusclnyj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2rpvjeqgr.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2brjzrcok.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2kldwpipa.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2mehvqyjm.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2zcpkjlcc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2ruuhcapd.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2biaorvaa.html


<!-- 参考信息 -->