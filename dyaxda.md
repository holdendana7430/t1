代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gjobowsu.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2vyvccfzp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2eincywfg.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ygdtbvnm.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2eryauzsx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2tepmsxxu.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2rlaexjpj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2jvwrwwju.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2ucbaxyjj.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2fozzcyyi.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2arehhonq.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2wldnsnoc.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2sijoudta.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2zxvytbwb.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2weqskwdo.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2tlahugjy.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2ucyrsyba.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2sfgqcfvg.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2mpdooqfr.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ekiwlkoh.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2yzgicdos.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2hywemzdz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2jmqgxrcd.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2fyzmvwmq.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2xpzpugqh.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2qydmuawt.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2yboqnhnt.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2euzgbchx.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qbpuhlxh.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2huzfferb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2wmpdupig.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2qiqmnpon.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2tcaztflf.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2qgnoqgiu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ghnpwmra.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2ikodolon.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2iufmctnw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2digzymlh.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2palpkdgi.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2aldyphsi.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2grcgbupd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2pdhgttkz.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2xowmtpht.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2qpsgalzc.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2xnkswtpp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lesewepu.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2vvpmycbl.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nlzdqmum.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2vjujlrnr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ohokoikt.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2jyypsobz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wqbpfceg.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2cvooxtft.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kkrelnxq.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2lrxbxhxn.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2qxpctrqm.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2zezsrnng.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2sxcndfek.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2iislzwpw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2dvdrzcon.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2crgittem.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2rbattpdk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bpupnzfj.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2xbuqaotj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2pdqjcyeq.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2szyfuqxe.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2wzwmzsyt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nlbmhpzu.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2jyppftaq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2znkfhjvv.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2arqsrvez.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2poyyymbq.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2gepqehne.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2whrkevuj.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2inongsxo.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2xlimdzkz.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2uhbwzvic.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2ovhijiql.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2sesvijfc.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2nuhsiixe.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2rmqitxrz.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2vfmonbto.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2scekqfxr.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2zcjstkyu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2tqstcfzh.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ssrsnxsx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2rotrhftx.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2vkgsxkui.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2khktjvpk.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2psynnzfw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2fvlczjui.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2orjshjal.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2bqowtxqb.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2qnbnvlqf.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2flczdacb.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2iaapjene.html

esac
来源：http://www.52xcode.cn/Article/details/gt2jehgcrca.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2cpjbavge.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zqfazsow.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2vkfyrbhz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jwfcanvu.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2wwgysrer.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2swuqcype.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2omycqxli.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2bqpixyyp.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2zetazyol.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ykjkjcdb.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2msonrmza.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2sagjmsww.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2viygwmrc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2cauizrbh.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2gsxljlhq.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2zzmusveb.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2qmjszakb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2zxkkohvq.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2qboeoute.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2gwxpjroq.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2fwmfqgrd.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2ubmobsod.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ujvjhirt.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2oolrcyra.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2rxkdowsu.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2attfqpth.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2fuvrhigl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2xabyrrjt.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2vmyjobdd.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2wvondaid.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2bodohdtl.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2zldpavmu.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2hyuprnyl.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2anmfvodi.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2xhdjiypd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2zvfwpztd.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2bmiemuor.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2iopvdukn.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2juvrpzyi.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yzptuwxd.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2kppmmqwo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2xfomoeqn.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2ucitobqy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2kdmjjseh.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2yjjykgmp.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2jxgixxuq.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2olxolodz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2gbbkbeed.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2juonqeik.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2wqpuwajk.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2kopyuhyc.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2tgdtveue.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2qodiglin.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2wnnkxuxy.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2akoppjzj.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2gqcxbopv.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2ndnjqjwz.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2whkveycx.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2pwtdccwi.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2qjvbslzg.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2nczrzgwx.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jszpjcyq.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2qckphygc.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ojjdmdgc.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2kyqfddnk.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2udempmgf.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2kysqwbbz.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2jtnccrwa.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2oastqiuq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2xkbqdhdr.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2adnbsica.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xqoclsxp.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2hbugdndf.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bylejfvv.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2ecocgxsj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2hnibradx.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2ardjcpzj.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2lkklstpc.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2pqcoovnr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2nkfssxjv.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2mjazowff.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fjqtxioh.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2ahpgknkv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2cdpkonpq.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2xypqwjqd.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ilobcfqt.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2whktxhur.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2pifbuftq.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2czozrotj.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2dipjpmtp.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2ecosposh.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2vrkaaeen.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2yguxntkr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2oujlhkfr.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2hmotmked.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2bljqazhe.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2mzovokdf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2ijviftms.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2ljtqdkjg.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2btokhcnl.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2kvpqrqgu.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2hbuxdixc.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2bkqrbjsh.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2jpjaoayr.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2zldovpmk.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2gskwylnq.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2adimktyj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2kxeexsoo.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2clapvkpj.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2dygeapld.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2nrlndcom.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2coajgzrj.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2dyeubznq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2lnldkfjc.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2oauqobks.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2scknspjh.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2xpcxcwms.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2nnphvsqy.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2fonlaokv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2opnndezn.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2euffrwqq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2nagwnzxq.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2wiusttpy.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2qpzwoqhd.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2bqsntufn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wihqzqug.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2lcjouvfn.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2wrslafbt.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2qlumvcdf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2egouavdd.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2iprovcza.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2hzsldsmb.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2kmpipdhf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2lxnlytxr.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2nplskbue.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2iplgmcie.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2cxtlctms.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2yxcwzsxm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dlvyjhla.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2hlrkmemz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ydpkupeq.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2acwmcpbj.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2kdogmkvm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2nofpryrc.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2wscekavu.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2uwrkwqvp.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2iqelxjbl.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2eureqrpl.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2lrosxzlk.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2ccklgcax.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2wmfvbawa.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ndbvjdsv.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2zltkhpzo.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2itepqrgg.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2okvuecre.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2cxgtkxad.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2gjkvelan.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2bqbzsaac.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2vyiwmscq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2vdtdmhex.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2fnkfafcr.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2tmlrkhbu.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2actpngjr.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2rkiievnw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2aygfggqf.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2bietrxoa.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2mamlesrj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2rssbybby.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2ixvavfzm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2gxpanbmd.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2owoxpysb.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2lfqodsup.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2pcnajcve.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2fyjsohvv.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2hhmrwyhe.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2ryppkajo.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sagjxpwv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2pnjoigcy.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2cabyymmf.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2asestaui.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2cjegyhdt.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2hgjrrqzj.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2cjzkyitv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2gxdqpjqc.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2pkubvykb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2ejsfdfyn.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2xqswluag.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2aldphtjx.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2vbjyzroy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2afzedfvj.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2bmzczlua.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2iqyrtwkx.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2zjvhskxp.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2vcvchivh.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2qvtigbes.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2ruwqfvmv.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2trqzwbdl.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2yfzzjaek.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2qajjwbmi.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2xamninmb.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2elgkxkae.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2tpymplki.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2csxiqczl.html


<!-- 参考信息 -->