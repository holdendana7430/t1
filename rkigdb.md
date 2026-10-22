代发 wailian999

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2zefutxpd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2obfuqwjh.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2bbsgokvh.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2aymkybbq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2oahdfqvu.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2xydseuok.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2fsuardcu.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2wtvmbsix.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2eggiktsk.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2tqdjzgiu.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2pveokfbo.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2fgrtpkmv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2kltienhy.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2tgwfjcnu.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2gytncnwg.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2jjkfelcl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2cglpktwx.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ywwtwlgx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ydhbbwje.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2dtwsmjud.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oxrdyqiy.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2vzimmtls.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rgraplwo.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2ozqhgmzp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dmhlsneh.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2uqaxbiqr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2srazpqhl.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2selgsnfr.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2dllsbafs.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2kkpiezuy.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2xwvmmgfo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2hrhsclot.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2xdjlmyeg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2blqhrlwq.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2pvqyypfl.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2jrtuvtvb.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2gbdftzlf.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2zxxjdbht.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2eipkyeow.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2ijsquizj.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2ebtpzndn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2ymxfifhb.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2xqzbjdlo.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2xiwkdvip.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2mefhpcyx.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2hbvljguo.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2klkkzykt.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2esgyeyyp.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2kbqazhqi.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2fhqbcjjt.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2ktcrztmr.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2cmdbocaz.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cpwhlpsk.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2dgkaogkb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2pvdyfmag.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2dmomwnlf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2chdjroba.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zrkldehu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2yazyvgar.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2nvspnejo.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2refvtitc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2wqnfyhhj.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2tfobhkac.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2jtubznhs.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2zcxbtuho.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2nacwsxre.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2jzahnivm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2ovkmjnso.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2zotgsjey.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jxzxbhej.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2abxuplqp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bnjndwmt.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2utdbtuzx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nrhjimhn.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2omfevndi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2anvndkuw.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2ztucavnm.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pmjjlvin.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2cxjoywfn.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2haxbbjkk.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2xfrdzkdq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2vdgxnfbx.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2ibxkpgct.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2ulgaujkk.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2iavqvvwv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2sretwwqf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rmsilxbu.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2lnevtame.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2xqlwttcu.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2wplszspw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2kvwhxbbx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zpkzftsx.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2sdzkvurq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sofoqita.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2hbunrpdw.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2sqbpkndz.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2swvukeyo.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2ktjjaneq.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2omlkcmfp.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2ojjmahxl.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2ergmvmqz.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2gbgrkqzg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2wqgykvci.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2tzzosrln.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2lebipsgl.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2wumlvynu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2afrphrte.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2ynlluinr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2iogjoybg.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2qzafltqn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2rvzfwicx.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ioiyxxwo.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2mswlyynf.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mvfrmamc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2iqyefvvj.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2abvtense.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2zwefcita.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2xesfkeri.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2qqhvksfi.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2wojofjcn.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2logunzlo.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2falzishi.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2jszzcaks.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2mqdgqbku.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2axwuulxu.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2ezawaiyx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2vetuvycx.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2abztthah.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2ppxihowk.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2tvtmofub.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2uytlgveq.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2mzdwnslf.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2zafskbav.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2dzcpirah.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2uwsmywld.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2pcbmarnl.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2kezepeeq.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2yckiiwvm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2umuixrsx.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2gjnfvezm.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2wplrkphj.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2gnewotuo.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2yhzbkffr.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2rxlmlvfe.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2dmpgjxuu.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2abugkhfn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ddiqcmne.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2ycnolcit.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2hflmepda.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2bmektdiq.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2snbptgqu.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2mpstmvfa.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2uuafnead.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2fllfcfkc.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2hivibwzf.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2odvvqccb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2uleaqhfr.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2gcdvaaec.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2oxahzqvo.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2fyyvdthh.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aaitaowo.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2ssdixhtx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2prpbjutx.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2ygeqqqpd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2vupkyrbr.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2lddfngql.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ojlwkpdm.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2tlgnzqpo.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2nxmdokdl.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2czdcaawg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2ljripnkd.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2ujgnqdjq.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2fxjxsfod.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2ppptjmpq.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2vhbvjijm.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2oqzxlwan.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2owkuxbwb.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2gpxgpkdc.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2dfotudqn.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2kxvguyku.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2tyyskfnt.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2nxdwfhgs.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2vsrjhvsz.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2qrygkbrn.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2vuldmbsp.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2hdjybnsw.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2dbymlpld.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2cgazpdym.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2comlusgb.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2jedmcwlm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2pbhiymxu.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2ejonnnti.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ryxlageh.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2toulmdrs.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2puievagf.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2uqgwwucd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2aocaqclk.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2ftfbahjx.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ykcbbydp.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2rbjrlbyz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2jryllfix.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2uuvhvqqx.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qebyivuq.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2wbkpptfb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2yuqeavvg.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2wqelxlms.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2ntnhrqxn.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2cafveykp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2ijmpzdqe.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2hitixwht.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2wxrwuqpl.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2phjpxzkx.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2ljcbyhao.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2nezuyidy.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2auaqivlw.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2lhjkimbj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2bnpyutas.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2gfsogvbr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2sdzqqucn.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2udghslgc.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2dmaorqac.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2gwixlljd.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2tweaupox.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2fnwgpyfu.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2cuabqkal.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2xdvgfoxa.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2mgrsvdhb.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2zvkqttwk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2euvpozoi.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2csdupart.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2xdcbtlkb.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2npulblox.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2jobkeecv.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2xrwmgjwu.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2avzpeeld.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2qyghmvsx.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2zvrxxbzz.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2lhwtayaf.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2mmmzjwux.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vzmzxsvu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2dwryxnvi.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2hztjczmb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2wxilhrmq.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2nmgngbhz.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2ziisifqd.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2anfgwrgn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2csixuykb.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2etgvstva.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2ldvpctup.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2grvezynw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2pwovhafr.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2lngrjzwh.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2pvrqofof.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2yjesxliv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2tlijqrep.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2ygvqsybh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2reuinayh.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2riascugw.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2qrrnxuqf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2poafoxxm.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2mynybppm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eessjzqa.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mtubifzq.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2nqffexhj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwutegiu.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2zwybhmps.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2jaycemuy.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2pfmicegz.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2ipithchm.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2zoitqqbb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2yfzajdco.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2uymstmwz.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2verpulfz.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2endbhzyv.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2xdxqrfuz.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2eukbckcd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2earjywif.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2yldnplsm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2cllojhxy.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2ndartheb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2dcrhbdoi.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2iyzobmld.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2zgzhgbac.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2soluhgoh.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2hxqkivhj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2imxxubkq.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2mbcgoupu.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2kzfpwhhx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2dpahtmki.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2jbtwxrjv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2kbccmcub.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2nsnztcvj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2ywvkawyg.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2spntnggf.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2ccrcjalq.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2gwnfopig.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2zqzikjdm.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2cdowxgte.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2mdokmyab.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2iyuysdyb.html


<!-- 参考信息 -->