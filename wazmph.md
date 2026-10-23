代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3qtfwfprq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3daraprff.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3fyaxvrbj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3nzxphief.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3jmtffqyr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3saejjhin.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3dzlgwdkw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3fvqlrmhu.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3sewchmtx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3gxjzwyja.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3ednerhxi.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3pvxfgrdt.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3rtidsxiw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3vjlzxtma.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3jljfzjdg.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3pnbkoqaq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3zfhqnoai.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3kfpofbmb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3tsybyuyt.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3csehkqyr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3rmmluopu.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3mbiytkiw.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ymxnascu.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3tdoesjqg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3jaartygv.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3znozaryl.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3pfehamiq.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3popnxxcd.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3alguhawi.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3amvgcdps.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3dcybwdft.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3iywnukhv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pdshqfiy.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3crqvssgl.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wnfnyrgc.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3rbaaryii.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xmmwtias.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3pkdazdzg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3vjxmgkko.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hpqykrws.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3qrivgkpm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xfdtoulq.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3aijshcjo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3drmqlknn.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3dknsyajk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3erejjbdu.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3gufmsdcd.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3oqicdfoc.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3pqmduobp.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3emrhwpls.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3wprvuzfx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3vuwhayye.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3rdutsjop.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3dlzocrfz.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3tzqrxbzu.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3drltybdl.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3zfrnsmzl.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3haiqilbx.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3qcwhlhrm.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3ibfhfqeo.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3zgfcfmgp.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3ckmvlgem.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3eplbroze.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3snxzpnbo.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wyqwvsjt.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3aibgmqud.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3nmpezgdf.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3fogwybme.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3amusibjw.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ftxrksfp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3akohohhh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3vriqbaig.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3flipakjj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3uipymnpu.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3asqtuhyc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3zqwlrvum.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3gbwfjpop.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3rpsolplv.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3mkcfwhbh.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3nqheylev.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3diamojkh.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bjzskoaq.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3zefevjgf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yzqaeqgd.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3apzgubnz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mttocqgb.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ioiojiup.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fklqoheh.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3uicmiipj.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vvxcfkhb.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3trbhvotr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3mhxygezt.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3oldperiz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3tikpddbf.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3rtdbjsjw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3shhwxoem.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3umbayszs.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3nwslwslp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qslorsbs.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3vochjolp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3vyedqoag.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3orfjmjuu.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3eutpxdrb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3juvmthvg.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3uznkvkcx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xqwymuhz.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3hpczcutl.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3tuhuxadk.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3qsfgfcsx.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3obwsgxeq.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3uohgpqtl.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3uiuywglt.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3lpujwckb.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3limomsnd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3febapuam.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3hwkxelew.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3enqhlzal.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3mdwbpxjo.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3vibghhos.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3cuxrahir.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3llseprvi.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3oewnpgvr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3kemevmee.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3sqfzzosl.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3xlkhucax.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3ophmxiae.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3wsvrvgld.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3ihdfblyh.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3ysucarqn.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3udefqnbk.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3xqxpwuxd.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ogxnnkmg.html

esac
来源：http://www.52xcode.cn/Article/details/gt3mplcqcxt.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3dijxjcod.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3djcuudgn.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3huwefcod.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ffnraeic.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3xefavmlx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ixyvhimh.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3pqymgjvf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3djsmnztl.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3cgegubjs.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3kiwqdgiu.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3cqwpgzft.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3xdcauxlk.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3pecyugdo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fznqmlnx.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3dhrlihch.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3yrzbxjxi.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3fyganssu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3aonbocsg.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3rotemvdv.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3lnimgldi.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3rdtyiebe.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3mmiffgfd.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3zwbydflm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3qkhfgmup.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3jpuwqwbt.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3jayohwnt.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3kwmkukow.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3ivntckcn.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3yrcgigcv.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3esgvlsjq.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3nbmuwwsv.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3griqihsj.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3jiipfhrt.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3wzkttwmq.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3bbeyibbx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3qjcahujg.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3woqhkrtw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3feaiccfn.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3sygwejkm.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3akcxwwhz.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3gpiavsgb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3mdnlnqqp.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3wkemdken.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3uhrhupuv.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3yycseaou.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3aupymgpg.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3tdqoqjhe.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3xeivtjwt.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3cbtyjwpj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3asbvfgky.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3dxxbwnqx.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3saqzeara.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3misgvtaq.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3ybwwomia.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3bwjtkvuh.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3etxkvwar.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3gchcajoz.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3fvhbnspl.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3kihgqjxr.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3lkioamjm.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3guzmvpcb.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3jksbiixr.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3spgcojgz.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3rqphdnjo.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3ijamviby.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3etnydvwb.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3phdgkful.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3beolvktp.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3cioiawcu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3yhtpispp.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3lmhswlln.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3bmkrkvyz.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3effwmahn.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3nxtdnxfp.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3gpxblhkr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3lbyduwis.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3jqbkxjnv.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3catulqov.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3hixlzxgx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3iarxnmkk.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3xfpucexl.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3qtrjtlcu.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3umtfwmcd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3yftlfjaf.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3avswunwm.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gavscndg.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3tytmczyl.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3digfyixq.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3brhojjft.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3ihrhpykn.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3rixyqtmg.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3xmeuoeik.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3dvqxuaie.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3toeuddeh.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3btvhzojk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3mdpirbed.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3gaguxrgl.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3fcczysng.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3cdarcgyk.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3dpirmrzf.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3saqgoziv.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3lennsiol.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3podydnwh.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3nijydkrn.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3hmezuhpb.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3fzrgzgoe.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3iuuelxjj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3erhfokqq.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3ejztsxfk.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3kxktuhnx.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3rgizgrxu.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3fzcjutuo.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3nnrapjqx.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nhemfyel.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3chdokuqf.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3wopfvsct.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3ozbticmu.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3wyappfmp.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3hnruutcm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3rggfggix.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3hybegodi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3lbdvqgve.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3nxgvovsu.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3kiiekjdv.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3mvqqfiye.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3ixrouweq.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3tskvjboc.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3vnjtqkzd.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3tlnomksf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3gleeodou.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3hzzppquu.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3xgapsxrw.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3dlyolsbr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3ksijopfx.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3tjjtewrh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3rrcicehh.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3nntjexlx.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3rvzvesko.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rxldzvnn.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3nutzousu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vodnxgtt.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bkgqvwic.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3lepsqndh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3nvswhsmz.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3andtcmlj.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3vitrbeeg.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3thyqcvgn.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3qvjtkpay.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3qwtdgvqk.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3pndytiea.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3lakaisue.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fayahmkw.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3gwwkitjl.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3lusyqxkj.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3cvnzwtxn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3bslemdjh.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3gjtirthk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3ecjcaoqh.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3wubkqirl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3vfozdnis.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3xduaelzl.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3ahvqtxoh.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rwgmjxkh.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3cemzoxel.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3jyqjcryw.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3yhkaudty.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3nwvuwwtl.html


<!-- 参考信息 -->