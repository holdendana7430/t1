代发 wailian999

[Q63] 开启事务
来源：http://wap.zdbjq.cn/Article/details/gwolscqyq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.hesvh.cn/Article/details/gzgqwgufe.sHtML

[Q64] 提交事务
来源：http://mobile.fehbvm.com/Article/details/gnidyzxrz.sHtML

COMMIT;
来源：http://www.blog.hesvh.cn/Article/details/ghkxvuylb.sHtML

[Q65] 回滚事务
来源：http://3g.hesvh.cn/Article/details/gbdanjacl.sHtML

ROLLBACK;
来源：http://blog.hesvh.cn/Article/details/gdgclaimd.sHtML

[Q66] 行锁查询
来源：http://read.share.zdbjq.cn/Article/details/grmhqbnqw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.hesvh.cn/Article/details/gewqtugxq.sHtML

[Q67] 设置隔离级别
来源：http://m.share.zdbjq.cn/Article/details/gwbyqiufj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fehbvm.com/Article/details/gvdkybgys.sHtML

[Q68] 保存点
来源：http://mobile.hesvh.cn/Article/details/galyghwys.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gmqkovicx.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gpxuzopeo.sHtML

[Q69] 查看执行计划
来源：http://read.share.fehbvm.com/Article/details/gqrnvvert.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.zdbjq.cn/Article/details/gscyooojl.sHtML

[Q70] 更新统计信息
来源：http://3g.fehbvm.com/Article/details/ggmcrpucz.sHtML

ANALYZE TABLE users;
来源：http://m.share.fehbvm.com/Article/details/gwwhbwaxo.sHtML

[Q71] 查看建表语句
来源：http://www.share.hesvh.cn/Article/details/gzgzfwxzi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fehbvm.com/Article/details/ggipgmrdm.sHtML

[Q72] 查看索引
来源：http://www.share.hesvh.cn/Article/details/gdnplfghk.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gpxopxcat.sHtML

[Q73] 查看表状态
来源：http://www.blog.fehbvm.com/Article/details/gmsxxsxiu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fehbvm.com/Article/details/gmsasushz.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/giafdfibd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.zdbjq.cn/Article/details/gyjyidpaq.sHtML

[Q75] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/ghdvewmgz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gzjyxhckr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/guukewhcj.sHtML

[Q76] 按天统计
来源：http://3g.fehbvm.com/Article/details/gtsygidzz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fehbvm.com/Article/details/gfuxoxgbg.sHtML

[Q77] 时间加减
来源：http://www.m.share.zdbjq.cn/Article/details/ggfbunlov.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.zdbjq.cn/Article/details/gzuecwwka.sHtML

[Q78] 当前时间
来源：http://wap.hesvh.cn/Article/details/ggqthgjxo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.zdbjq.cn/Article/details/gotpyejhw.sHtML

[Q79] 字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gepyixdso.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fehbvm.com/Article/details/geqiqzhwz.sHtML

[Q80] 字符串截取
来源：http://m.share.fehbvm.com/Article/details/gjqcstoel.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fehbvm.com/Article/details/gqbujapzx.sHtML

[Q81] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gocfbtsuu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fehbvm.com/Article/details/gjwrnapjr.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/gvcambudw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gyononpdm.sHtML

[Q83] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gehswrbnw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gexmaoyfu.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fehbvm.com/Article/details/ggxuzsdsg.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/ggfgopzja.sHtML

[Q85] 数值取整
来源：http://www.blog.zdbjq.cn/Article/details/gqygsamda.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.hesvh.cn/Article/details/gbmklpwtq.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fehbvm.com/Article/details/ghryvegnq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.zdbjq.cn/Article/details/gdbuecdwh.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fehbvm.com/Article/details/goeztjtft.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.hesvh.cn/Article/details/gftzbsvqz.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.zdbjq.cn/Article/details/gudmepzkq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fehbvm.com/Article/details/gktllfdds.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gwafgtbly.sHtML

[Q89] 判断表是否存在
来源：http://3g.hesvh.cn/Article/details/grqgjkkqw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gyzizdpjk.sHtML

[Q90] 生成序号列
来源：http://3g.zdbjq.cn/Article/details/gijhmhgez.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.hesvh.cn/Article/details/guyeedmls.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/giaseyalo.sHtML

R. Bash 专题
来源：http://m.share.fehbvm.com/Article/details/gfkdmzxmy.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gojnzplxb.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.zdbjq.cn/Article/details/gmshgkczd.sHtML

#!/usr/bin/env bash
来源：http://mobile.fehbvm.com/Article/details/gdzaagqun.sHtML

set -euo pipefail
来源：http://www.share.fehbvm.com/Article/details/gfsydknzz.sHtML

[R02] 变量赋值与使用
来源：http://wap.hesvh.cn/Article/details/gqpfsuoaa.sHtML

name="Tom"; echo "$name"
来源：http://baike.fehbvm.com/Article/details/gnmqmlhql.sHtML

[R03] 只读变量
来源：http://blog.hesvh.cn/Article/details/gusjbzite.sHtML

readonly PI=3.14
来源：http://mobile.fehbvm.com/Article/details/gcorvfqro.sHtML

[R04] 位置参数
来源：http://read.share.fehbvm.com/Article/details/gdlqncuwl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.hesvh.cn/Article/details/gfskyyukn.sHtML

[R05] 参数默认值
来源：http://www.blog.fehbvm.com/Article/details/gjritqmtv.sHtML

name="${1:-default}"
来源：http://www.blog.fehbvm.com/Article/details/geyedrgaz.sHtML

[R06] 判断命令是否存在
来源：http://www.share.zdbjq.cn/Article/details/gubrmhptj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gbltewbdo.sHtML

[R07] if 判断文件
来源：http://blog.hesvh.cn/Article/details/gumnagupe.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fehbvm.com/Article/details/ginjrmdjh.sHtML

[R08] 数值比较
来源：http://www.blog.hesvh.cn/Article/details/geuljigzf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.zdbjq.cn/Article/details/gpttmafyn.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gjikloojh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.hesvh.cn/Article/details/gzlfeptcz.sHtML

[R10] 正则匹配
来源：http://wap.zdbjq.cn/Article/details/geblnnubz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.hesvh.cn/Article/details/gmrigffhj.sHtML

[R11] case 多分支
来源：http://wap.hesvh.cn/Article/details/gyvdbppvj.sHtML

case "$1" in
来源：http://read.share.fehbvm.com/Article/details/gnksqtlzn.sHtML

start) echo "启动" ;;
来源：http://wap.fehbvm.com/Article/details/gkicqwuod.sHtML

stop)  echo "停止" ;;
来源：http://wap.hesvh.cn/Article/details/gfcntdifb.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/ghkkbrgji.sHtML

esac
来源：http://mobile.hesvh.cn/Article/details/gletemscv.sHtML

[R12] for 遍历文件
来源：http://3g.zdbjq.cn/Article/details/giimxzfgo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.hesvh.cn/Article/details/gcdgnxkki.sHtML

[R13] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/gocahudjv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/ggszjpooq.sHtML

[R14] C 风格 for
来源：http://baike.zdbjq.cn/Article/details/gsibhxcdk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gyvfrnycn.sHtML

[R15] while 逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gyrhfamjx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gakdaftxv.sHtML

[R16] until 等待条件
来源：http://mobile.fehbvm.com/Article/details/gqjdfhvre.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gpndxqwbp.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fehbvm.com/Article/details/gbcuquznx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/gelwztqbr.sHtML

[R18] 遍历数组
来源：http://www.share.hesvh.cn/Article/details/gswhoqvjj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/gxzisuprm.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gfwtzlirk.sHtML

echo "${#arr[@]}"
来源：http://mobile.hesvh.cn/Article/details/gdjapubla.sHtML

[R20] 关联数组（字典）
来源：http://blog.fehbvm.com/Article/details/gzdfoihnh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/gifztcvps.sHtML

[R21] 字符串长度
来源：http://baike.zdbjq.cn/Article/details/gimuyezlb.sHtML

echo "${#s}"
来源：http://www.m.share.zdbjq.cn/Article/details/ghqtgejfb.sHtML

[R22] 截取子串
来源：http://baike.fehbvm.com/Article/details/ghrqeesbn.sHtML

echo "${s:0:5}"
来源：http://mobile.zdbjq.cn/Article/details/gqyewitab.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gpshfoqyr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.hesvh.cn/Article/details/geeacfgag.sHtML

[R24] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/grkuxocwy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.zdbjq.cn/Article/details/gfcwfwdjl.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.hesvh.cn/Article/details/gjhqyroyw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.hesvh.cn/Article/details/gtgavrkhx.sHtML

[R26] 命令替换
来源：http://read.share.zdbjq.cn/Article/details/ggjhpqlkn.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.zdbjq.cn/Article/details/gwmvnplml.sHtML

[R27] 算术展开
来源：http://wap.hesvh.cn/Article/details/gmnoudguk.sHtML

echo $((1 + 2 * 3))
来源：http://3g.zdbjq.cn/Article/details/gbtyglskc.sHtML

[R28] 浮点运算
来源：http://www.share.zdbjq.cn/Article/details/gfqjhkufx.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fehbvm.com/Article/details/gqzkozxlz.sHtML

[R29] 定义函数
来源：http://www.share.fehbvm.com/Article/details/gmqxhkorr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fehbvm.com/Article/details/gnfngnntt.sHtML

[R30] 函数返回状态码
来源：http://baike.hesvh.cn/Article/details/gwyxiavqt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fehbvm.com/Article/details/gtbepkdol.sHtML

[R31] 局部变量
来源：http://wap.zdbjq.cn/Article/details/gvblzycfq.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.hesvh.cn/Article/details/gyqhndykl.sHtML

[R32] 参数个数校验
来源：http://m.share.hesvh.cn/Article/details/gdvqicevz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gogcltmco.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.zdbjq.cn/Article/details/gzbydnspo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.hesvh.cn/Article/details/ggyufixiy.sHtML

[R34] 退出时清理
来源：http://m.share.zdbjq.cn/Article/details/ggdpsramm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/grgjcntnr.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/glokgqrql.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.zdbjq.cn/Article/details/gfuqmpfzm.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fehbvm.com/Article/details/gniojrtei.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.hesvh.cn/Article/details/gylmrpent.sHtML

[R37] 把输出赋给变量
来源：http://read.share.zdbjq.cn/Article/details/gixtodiia.sHtML

files=$(ls -1)
来源：http://baike.zdbjq.cn/Article/details/gmogcrcde.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/gnigqdiel.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/gkqaxtuti.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fehbvm.com/Article/details/glistvysv.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/gavgzkivi.sHtML

[R40] 追加写日志
来源：http://3g.fehbvm.com/Article/details/gwjdjphds.sHtML

echo "log" >> out.log
来源：http://www.blog.zdbjq.cn/Article/details/guncuwkvw.sHtML

[R41] 丢弃输出
来源：http://mobile.zdbjq.cn/Article/details/gvaehkjfr.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gmgeascge.sHtML

[R42] 输入重定向
来源：http://wap.fehbvm.com/Article/details/ggurwphev.sHtML

wc -l < a.txt
来源：http://read.share.hesvh.cn/Article/details/gjdsffvcr.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/gxfaltgmq.sHtML

find . -name "*.log" -type f
来源：http://wap.zdbjq.cn/Article/details/gobmnfjnk.sHtML

[R44] 按修改时间查找
来源：http://www.blog.hesvh.cn/Article/details/gvwogrlvq.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/gtcqhiogo.sHtML

[R45] 批量删除
来源：http://m.share.hesvh.cn/Article/details/gfobucmol.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.zdbjq.cn/Article/details/gpmyetyjr.sHtML

[R46] 递归替换文件内容
来源：http://blog.hesvh.cn/Article/details/gkmygxbfw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.hesvh.cn/Article/details/gqlmmagul.sHtML

[R47] sed 单行替换
来源：http://m.share.hesvh.cn/Article/details/gvizcctbe.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gzlsclnbx.sHtML

[R48] awk 取指定列
来源：http://m.share.fehbvm.com/Article/details/gziutlvyc.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gxwocasab.sHtML

[R49] awk 带条件
来源：http://wap.fehbvm.com/Article/details/gmlakrdrx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fehbvm.com/Article/details/gtjruhkzr.sHtML

[R50] awk 求和
来源：http://mobile.hesvh.cn/Article/details/gmofzickx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.hesvh.cn/Article/details/gyjppkiyi.sHtML

[R51] 排序去重取前几
来源：http://www.blog.hesvh.cn/Article/details/gugjvhalf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fehbvm.com/Article/details/ghekqrclj.sHtML

[R52] 统计行数
来源：http://baike.fehbvm.com/Article/details/gxmclemcc.sHtML

wc -l a.txt
来源：http://mobile.hesvh.cn/Article/details/gqcfbojgm.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fehbvm.com/Article/details/gccgkfnru.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.zdbjq.cn/Article/details/gzovsdvfu.sHtML

[R54] 比较两个文件
来源：http://read.share.hesvh.cn/Article/details/gazgphtbk.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/gzikxvhbu.sHtML

[R55] 压缩与解压
来源：http://www.m.share.zdbjq.cn/Article/details/gllxeqwci.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/gynocdkqx.sHtML

[R56] 远程拷贝
来源：http://blog.zdbjq.cn/Article/details/ghxofksci.sHtML

scp file user@host:/path/
来源：http://m.share.hesvh.cn/Article/details/gvadsavpq.sHtML

[R57] 远程执行命令
来源：http://read.share.hesvh.cn/Article/details/gapqwzdnv.sHtML

ssh user@host 'uptime'
来源：http://mobile.fehbvm.com/Article/details/gpqbrupqf.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/grnhaqkev.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fehbvm.com/Article/details/gnktfosvi.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/gueyhfzbc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.zdbjq.cn/Article/details/gkqkamndc.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/ggwumarmx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fehbvm.com/Article/details/guhxnnyoo.sHtML

[R61] 磁盘占用
来源：http://read.share.fehbvm.com/Article/details/gghulqozj.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/gjltehsmf.sHtML

[R62] 找最占空间的文件
来源：http://blog.hesvh.cn/Article/details/gcshjtjge.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gtjrtwxil.sHtML

[R63] 内存与进程
来源：http://m.share.zdbjq.cn/Article/details/gvqmzcoia.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fehbvm.com/Article/details/gtsqyises.sHtML

[R64] 结束进程
来源：http://www.blog.hesvh.cn/Article/details/gsqatekqv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.hesvh.cn/Article/details/gnvnoiazq.sHtML

[R65] 查看端口占用
来源：http://wap.fehbvm.com/Article/details/gcppzkdlj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/gpkplipae.sHtML

[R66] 定时任务
来源：http://www.share.zdbjq.cn/Article/details/gdtqxrvhq.sHtML

crontab -e;  crontab -l
来源：http://www.blog.hesvh.cn/Article/details/gojoosdfu.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fehbvm.com/Article/details/goavvzigh.sHtML

openssl rand -hex 16
来源：http://wap.zdbjq.cn/Article/details/gemkjlmdu.sHtML

[R68] 计算文件校验值
来源：http://m.share.zdbjq.cn/Article/details/gfxoptqiz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.hesvh.cn/Article/details/gpiynzoly.sHtML

[R69] 生成随机密码
来源：http://wap.hesvh.cn/Article/details/gjfattyio.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.hesvh.cn/Article/details/gvvcnbnsb.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/ggkbsaukt.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.zdbjq.cn/Article/details/gcbrmctob.sHtML

[R71] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gnaipanhs.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fehbvm.com/Article/details/gnnlpjyny.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.zdbjq.cn/Article/details/gczfmlgac.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/goyqydhrn.sHtML

[R73] 分割大日志
来源：http://blog.zdbjq.cn/Article/details/gytpxnfbq.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/gvjbgtura.sHtML

[R74] 批量重命名
来源：http://baike.hesvh.cn/Article/details/gvqbywcvb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fehbvm.com/Article/details/gyfnvrwwp.sHtML

[R75] 导出环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gwpmgkwhx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.hesvh.cn/Article/details/gwmupfcpg.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/gdyclsftv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gjpryuukw.sHtML

[R77] 读取用户输入
来源：http://www.share.hesvh.cn/Article/details/gyhpmrmfb.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/gkuzqcxqj.sHtML

[R78] 交互式菜单
来源：http://wap.fehbvm.com/Article/details/gwttkigon.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fehbvm.com/Article/details/gncsdlupc.sHtML

[R79] 解析命令行选项
来源：http://mobile.fehbvm.com/Article/details/ghpmihezx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.hesvh.cn/Article/details/ghrwzwype.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.zdbjq.cn/Article/details/gxtogbsny.sHtML

time ./run.sh
来源：http://read.share.fehbvm.com/Article/details/gygbtajfv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghqbpaaqc.sHtML

S. C / C++ 专题
来源：http://baike.zdbjq.cn/Article/details/ghzhzkmlj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/geauoptlg.sHtML

[S01] C：Hello World
来源：http://baike.fehbvm.com/Article/details/grnubxtop.sHtML

#include <stdio.h>
来源：http://www.m.share.hesvh.cn/Article/details/gagmaoswh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fehbvm.com/Article/details/gamfzfhya.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.hesvh.cn/Article/details/gftvjkmgx.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fehbvm.com/Article/details/gzwippink.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/gnlwrnxif.sHtML

int x; scanf("%d", &x);
来源：http://3g.zdbjq.cn/Article/details/gafauhkzr.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/gjybqbmwf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gqkiuioyp.sHtML

[S05] C：字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gqsdaahpj.sHtML

strlen(s)
来源：http://blog.fehbvm.com/Article/details/gjktzagje.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/gcfhgsauh.sHtML

strcmp(a, b) == 0
来源：http://wap.fehbvm.com/Article/details/gvlbmcfra.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fehbvm.com/Article/details/gwvfgkzjw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/gpoedanxl.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.zdbjq.cn/Article/details/gdhrjzdcz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.hesvh.cn/Article/details/gswdllkww.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.zdbjq.cn/Article/details/gwtqwdowb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.zdbjq.cn/Article/details/gucrxnyrx.sHtML

[S10] C：指针与解引用
来源：http://read.share.zdbjq.cn/Article/details/glqbusfal.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fehbvm.com/Article/details/graxdzldj.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/grjftlsri.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.hesvh.cn/Article/details/gejsugwkl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fehbvm.com/Article/details/ggxcttvbt.sHtML

fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/ghapahymy.sHtML

[S12] C：写文件
来源：http://blog.zdbjq.cn/Article/details/ghcncpzdh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/giifsnjct.sHtML

[S13] C：宏定义
来源：http://read.share.zdbjq.cn/Article/details/gmdvrkzef.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.hesvh.cn/Article/details/gxfzivfbp.sHtML

[S14] C：枚举
来源：http://blog.zdbjq.cn/Article/details/geehlxixy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.hesvh.cn/Article/details/gdnpekmni.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/gfmpafrqs.sHtML

(double) a / b
来源：http://wap.fehbvm.com/Article/details/gnrnzsmxu.sHtML

[S16] C：位操作置位
来源：http://www.blog.hesvh.cn/Article/details/gqqfqzddy.sHtML

x |= (1 << 3);
来源：http://blog.hesvh.cn/Article/details/gjplotauo.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gkxilbmve.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/gqlemjpzm.sHtML

[S18] C：命令行参数
来源：http://baike.hesvh.cn/Article/details/gbeeytcfi.sHtML

int main(int argc, char **argv)
来源：http://mobile.hesvh.cn/Article/details/gvnkhdcdq.sHtML

[S19] C：快速排序
来源：http://www.share.hesvh.cn/Article/details/gipppfimd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gifsvgrxp.sHtML

[S20] C：二分查找
来源：http://baike.hesvh.cn/Article/details/ghrbxoddt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gdasntvea.sHtML

[S21] C：字符类别判断
来源：http://www.blog.hesvh.cn/Article/details/gqfpnqmyl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.hesvh.cn/Article/details/gspuqioxq.sHtML

[S22] C：字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/grlgacytg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.zdbjq.cn/Article/details/gueplqjzu.sHtML

[S23] C：随机数
来源：http://www.blog.zdbjq.cn/Article/details/gpzuupppd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.hesvh.cn/Article/details/gwomjwsqf.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/gzmkxtumz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gigadncxf.sHtML

[S25] C：内存拷贝
来源：http://read.share.zdbjq.cn/Article/details/gygvwgkbn.sHtML

memcpy(dst, src, n);
来源：http://www.share.fehbvm.com/Article/details/glheqafns.sHtML

[S26] C：内存清零
来源：http://www.m.share.fehbvm.com/Article/details/gmpcmaxer.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fehbvm.com/Article/details/gpohfupff.sHtML

[S27] C：定义常量
来源：http://mobile.hesvh.cn/Article/details/gpacpgzrc.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gypfkigli.sHtML

[S28] C：静态变量
来源：http://mobile.zdbjq.cn/Article/details/gfnhhmlpq.sHtML

static int counter = 0;
来源：http://m.share.hesvh.cn/Article/details/gnpeieowj.sHtML

[S29] C：变参函数
来源：http://www.m.share.hesvh.cn/Article/details/gwebpmbxl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fehbvm.com/Article/details/gdrojjlrv.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gjgsckvte.sHtML

#ifndef X_H
来源：http://blog.hesvh.cn/Article/details/gqgdevjid.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/gwnluawoe.sHtML

#endif
来源：http://3g.hesvh.cn/Article/details/gynqvskkw.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/gcigsrqtd.sHtML

#include <iostream>
来源：http://www.m.share.hesvh.cn/Article/details/gocucemdk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fehbvm.com/Article/details/gudzzxinz.sHtML

[S32] C++：字符串
来源：http://mobile.hesvh.cn/Article/details/gkztafjum.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/gtxguiuuh.sHtML


<!-- 参考信息 -->