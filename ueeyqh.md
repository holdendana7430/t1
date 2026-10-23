代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3xomcsbao.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3ezxvpxlv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3bptuawcm.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3ntvqwfzf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3pmbowlcj.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3qrjrhwnk.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3deyphygo.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3hxswkkbc.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3bhsgcish.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3nluexvrv.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3ufdcrelb.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3wqcpfkth.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3gwzxwqhj.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3mmuieuoj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3amadegah.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3wssckikl.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3byquhqvg.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3ldaoutrr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mgvznmpn.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3hnnkngcz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fwlearaz.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3jjcdrygt.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3spqdosax.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ofyxrkjw.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3zphudxwz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3lmxiacxm.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3zvreguuq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3wrmmyhjm.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3dxgnppfs.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3sgvnosar.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3ovlucvsp.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3efskzaou.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3techfzcl.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3ywealdwy.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3jrrnolnq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3pglkeaoh.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3zwqnmkpp.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3ypfitidc.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3zygastfh.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3nscyweoe.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3khgplxjv.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3pysgjugn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3wtpmccoo.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3ggelygwn.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3tuhwqjiy.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3sdrakqgt.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3acptjfda.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3ezraebpj.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nqwdgsqp.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3vivyfovz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3wonyfqxs.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3mekpwina.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3rdszqmex.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3yiemyxsf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mfaivhcl.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3afworhlf.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3ibnpsjbu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3osgdgodw.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3tumoryxb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3alsplowe.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3lrwsudnr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3rnnvtncz.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3zhugehcw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3xswatpso.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3qqqkjoqq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gthyploa.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3pcqzbswa.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3crnyawrd.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3fvzncbei.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dzvaktst.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3vcyyqyvi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xotyjvtm.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3lnrkrkcc.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xdrmtzsr.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3kuhdqbhe.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3uovoajyv.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3ftosyxhd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3wzucplcm.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3ppqyltrd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3tnoqausb.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3yxukazwo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3lptpnjof.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tqcbjaha.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3yvbuvspc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3mdrubfdy.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3wqtixien.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3mgzqfjhc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nnfjhyxf.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3ceskvumc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rftwsnfj.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3iaglfbbf.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3oeoauiao.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3tecnlwne.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3wruagwoe.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3pxwtnvda.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3jgdarcav.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3wwpgbtho.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3fygowsyq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3eecvmqjp.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3qapzelww.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3cqakrxqq.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3csqolrad.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3guxtpxje.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3eismsljk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3cchomvhj.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3gmgncukh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3jfkjoqrb.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3disfpwfq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3pxroptte.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3fyizonsy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3uhngoocu.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3manaatwp.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3gkfzlkxj.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3jekmurcl.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3afgudies.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3pfdhrggy.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3pwivlzie.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3jolqphvf.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3lwooksrd.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3gcqtfwwb.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3iumlkgpx.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3zruilckg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3lozddbwu.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3krqmuenv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ooivsvpo.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3joyjmreo.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3cyvesiwi.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3sevsuiio.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3bstzsqrm.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3nhuckzeh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3jafdvwxv.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3pcwnhpmw.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3smegnomd.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3awupljuj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3edfmkbid.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3erywojle.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3jirdgvpt.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3crgjimzd.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3qszeufmk.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3wtjhaywm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3bbjgijpv.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3dpiqdguz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3qyafqsoe.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3kxcqxfvg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3tqwiajlf.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3zltpqudl.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3mqarkgrq.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3zlfjcqrp.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3pdhjboxm.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3gbtvmmrq.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3smymqccn.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3epqxvuxi.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3hmphyqsu.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3usiklzst.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3kkgwrinw.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3vpzaeqnm.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3vqrzeqpx.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3kzjxfcrd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3hncqrlcz.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3fmkyujyu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3trmmusmf.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3ovlhjrov.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3jlpwhkno.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3iomxjxxp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3zvtzprib.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3qatdxlbg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3gjftseal.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3ukwqhqdh.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3vnuroyed.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3xburexjr.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3qbihxxzt.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3bjgpbzxw.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3vgfspvhf.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3ulpoimhf.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3eywdpawu.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3enylojwx.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3duwimchs.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3eqanoqlp.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jmovutyf.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3pbabczfv.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3bdsjrzsn.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3lxunohuv.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3tkqlsvly.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3ozfwrfhx.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3lllopedn.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3wgyodchc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3bogvbnwe.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3kgiqbbiu.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3cqhcagce.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3sglayyuy.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rifjckns.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3rmzornjy.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3vrauqdhj.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3kmjnjjyh.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nwfjjwlp.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3ljqqekkb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3lpcerpum.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3taoxagol.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dmrmpgzx.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3uzhbmrrk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3fcvozpab.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3lltxcokz.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3bbewxnab.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3yavdauww.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3pozcbild.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3hkkaeqjo.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3yjglhgni.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3ywhrtcpe.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3dpxlvauh.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3ftakmcaz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3svvvojqv.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3lnuykjlm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3sceuiusv.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3vbxsyulx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3stnaihvx.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3bcsysvsz.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3kzsojggi.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3wdpazuoh.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3upizflow.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3njelvfbi.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3twfoluya.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3snvfkppr.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3ecraifie.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3ckyvlvxz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3oebyxdmi.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3ssjrheys.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3kqqzncru.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3tzcsqmrf.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3gkbvaaaf.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3mcdxodbx.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nffmckmz.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3uytpucvv.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3gdzcgwfi.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3oimpnhtz.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3oonbgsvl.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3zuseroob.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3ildzawvm.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3iqutrcpf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3eitlogmu.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3nwltpaqh.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3cmrducbe.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3xjohzrja.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3pzlslupi.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3gpfkffot.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3ncihokoh.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3chascccn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3cwohvmrq.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3idmtpnoa.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3rgnpwjgd.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3tdzkbokb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3zjivqrxc.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3woddnrzo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3pbytvmat.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3accgfiby.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3mfknlgac.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vboethdi.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3eikopeoo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zpbdhmqa.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3asttgvai.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3jbmpxntg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3xipywwnj.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3owjmboss.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3aknpwxnh.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3qqrwtkfb.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3jldbzbod.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3frbjzftd.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3aqkipwjy.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3tomiefve.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gpltbfiu.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ztgdhxrr.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3gefcxtkm.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3ogricvta.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3bhxlsazf.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3laoyeiyp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3urxoiiof.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3eygzngzo.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3dpopgyie.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3bfsikqar.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3tonhzqet.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3hzktmssi.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3fyklakew.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3belkzxnr.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3rzciwptc.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3yexlfjcb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3pfdixmtp.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3lrfxotha.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3hagzjycy.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3pkjyawje.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3ihukingl.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3hovjceoh.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3cljsomre.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3vrhvzblm.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3suqgrxtl.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3snzuiref.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3lbaipbjd.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3bpjceolm.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3lxlbdpui.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3fixxbyiz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3yhxsxxdy.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3tclyrrak.html


<!-- 参考信息 -->