代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3flvufoww.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3cbuqifth.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3trghftxl.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3isdtfehj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cnboytom.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3tazhpjec.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3aopikswt.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nqgviqpp.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3mlizmvth.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nftoqpyv.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3sixihnre.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3pnowqzgy.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3fgxzouya.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3kfxmpnml.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3rcwklcrh.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3htnlfhqd.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3errslqag.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3cwhkhcbt.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3jxjgfvci.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3ljrvjtuh.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3tssxstsu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3gfjmjroj.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3djjbqdzv.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3hxsodqnw.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3iukyuhan.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3fwerlodw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3duktghkn.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3jwhdawen.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3lnjgymni.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3dmpuqyhz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3rlksmtjw.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3wyfzbvfy.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ajtldcya.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3plgbdvrn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3gshcdqvf.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3likjfqrc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3nvpjvagw.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3yjplgtmt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3phpptafg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3ksellkyo.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3ysauabde.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3nvvqkkcq.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3gptveigm.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3vkrrgwmg.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3zuhunapu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3agylwgnc.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3dikuyemw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3tnbjalax.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3yzubqesl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3exyiqjoy.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3quxjzybu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iijpwuqh.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3mxrbwlwj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vudtmmcy.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3vjcmnszy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ovhjyira.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3vanqjkfz.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vrsvvdhp.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3udrrowgm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3rkeeiqgq.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3mnwgcrlq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3zjbnnoqx.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3wmkprafy.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3uarkyhhn.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3xpfepnar.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3enwqcfox.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gnkozplp.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3qlowmonv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3ppnzqiut.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3ivmbelyh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3gdgupwep.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jmynzmwq.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3fmyodrfe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lwcjmijp.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3loujdopq.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3dyqddbte.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3udimzcvt.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3bnusdgce.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3vmwosrqh.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3cepmilzb.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3tveuezrb.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3kquhounp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3ktxjtxri.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3vkbxylsq.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3equnaszh.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3lkaktgsv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3cimauiqd.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3ayqdwnkx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3hwnfphat.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3kqkkffbt.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ywznabex.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3aowoaqvw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3suijqwwn.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3iyyrbgzo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3xeytorra.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3vlrdcaug.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3bocvnedh.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3qrgyoxre.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3okuzqxso.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3obtxlgmd.html

esac
来源：http://www.52xcode.cn/Article/details/gt3djzhzlrm.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3zfmtytfc.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3phfdlwlz.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3zbjrzcca.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3vejhqnpb.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3zdktdaee.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3nvxkevcj.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3rppgtvmu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3zfirlltg.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3hgohwaoz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3aivkgzsq.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3hgdkurpo.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3ymyhtodb.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3ozopoffi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gcdiencm.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3niufwqbl.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3bzwudwgb.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3ljwrevzb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3uedcdaky.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3vpujvkfv.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3dhtdbusd.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3uheuzwlc.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3ocrmlanl.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3blsjjwvv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3bhlypdty.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3rwpjlubv.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3svsdycyu.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3oyzkuxui.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3ofxjwxwc.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3mgzptszv.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3lnkbxugx.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3cvyaijjq.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3ppghqmnp.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3rnprmjhn.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3ivnipklo.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3jrybjkgy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3yfcjsnjn.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3gtumbiux.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3hwtzbkjm.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3fqpctbkl.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3zivmbljm.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3brpvsrfm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ectzsrwv.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3ykpjtwhy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3icrwiwjv.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3nfdwnizr.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3jhllqfis.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3hrjlfyym.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3vyujjzhg.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3mbagryfc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3jvcbaocb.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3tveoylnb.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3rfkaqlpz.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3uqikpfnq.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3elzfzntn.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3vpbrjahz.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3jacutiwt.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3reckcjnu.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3xiowltuv.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3jwcpierj.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3kacdjiey.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3jnlebbne.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3owzysqtb.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3jwqqsvru.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3xaknjoiq.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3tobkktzl.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3lnxqzrbz.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3qvjcrqng.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3qekrqpqz.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3lngjuuvq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3tpiuzoub.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3btpbwbgu.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3gvofhdjt.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3hmqzqhtg.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3jcjehvhb.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3ljlvchxs.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3uhvhtrci.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3edsjwsfu.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3eqkkepny.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3btmqabss.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3aiiygnpr.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3bplheajf.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3buhjlzel.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3ohjerelc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3dgrbcivf.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3jhqziete.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3tibpxrtd.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3tfzrtooh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3zamdfmgg.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3wnsstkma.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3ouqjzukl.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3ttqxqsmq.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3tjgcbrdo.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3ogtvdrif.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3gurlbrxp.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3wdlabuvj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3cwnuxlob.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3uwfmltor.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3msnsajoo.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3sfbyocmh.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3xjkhslak.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3qibesliy.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3azglmqlx.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3cjsgunty.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3ghwbhkwg.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3oeyxwzok.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3mbpwzdhj.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3yfbpprpr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3marzrtju.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3ixocqfve.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3ixhxhsli.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3xagvkecp.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3vgrajozt.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3hojdxqoi.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3yvitnrlu.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3kmsgenqa.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3iitaoqdg.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3lyhecejm.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3qzqrooqq.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3psvolfjd.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3ycidwoai.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3dqdtootv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3kwkdhgfd.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3aqcfrynm.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3ruqzuwuj.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3ulpbswtw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3glsxojzu.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3pdbslbbl.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3drchxmgc.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3tpksfvkw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3uutoastt.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3egggjiqa.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3qkxflukb.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3rwmergyh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3ejydmsfy.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3ztapjxsn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3cuklubrk.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3egdmmrys.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3aexkkhzq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yfedzutu.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3ysnxhjkr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ftjrzpae.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rlbdkhvl.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3ughxflxh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3zecnrrlq.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3xjcfaskv.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3zuqpbvxc.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3vgtbvtvj.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3wovwhgck.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3hmpurykp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3mladuztp.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3difqjwyl.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bzryfrlz.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3chvodsvm.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3huxkauti.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3bqxrozbq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3atddamdo.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3qmwjlvcg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3sajpdfzq.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3qofbmjup.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3qyenvhle.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3iozjfgcs.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3vafnhvme.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3kscxuwju.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3klquvtfp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3exlxoyfq.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3sihxmmqq.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3watjmlja.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3yitvraoi.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3zztwtcfh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3fsdwfobj.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3wrbqysbm.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3zxgvzrxl.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3uypvoorq.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3bjvkzfty.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3fjxtiuiz.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3cndxmmit.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3xcxcsepb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3mpluxjcq.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3iznmmqum.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3vcqpqoup.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3jxdjuptg.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3kcigclff.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3lstbpkhf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3zynclkcx.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3aykbzpjy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3liykrhja.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3ohgyqjhl.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3cybhusrt.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3tkzeclzx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3eebsdsll.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3egebqcif.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3usddydrj.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3qrstjtko.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3tntvzasj.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3pynvoins.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3cylzhmaf.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3zujjwmxh.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zrpiqlls.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3tnjwlqyk.html


<!-- 参考信息 -->