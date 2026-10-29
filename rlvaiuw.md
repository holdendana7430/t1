代发 wailian999

[Q65] 回滚事务
来源：http://mobile.zdbjq.cn/Article/details/gjdwpcnqd.sHtML

ROLLBACK;
来源：http://m.share.zdbjq.cn/Article/details/gehwzwyuf.sHtML

[Q66] 行锁查询
来源：http://www.m.share.hesvh.cn/Article/details/grtmpdulh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.hesvh.cn/Article/details/ggvjhjpro.sHtML

[Q67] 设置隔离级别
来源：http://m.share.hesvh.cn/Article/details/gxcrqlqhp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fehbvm.com/Article/details/gmciawmyp.sHtML

[Q68] 保存点
来源：http://blog.fehbvm.com/Article/details/gaketyvhn.sHtML

SAVEPOINT sp1;
来源：http://mobile.zdbjq.cn/Article/details/gnuhoxhlw.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gfwsidhiw.sHtML

[Q69] 查看执行计划
来源：http://mobile.zdbjq.cn/Article/details/gshmpdqnf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.hesvh.cn/Article/details/gwxbdtogt.sHtML

[Q70] 更新统计信息
来源：http://baike.fehbvm.com/Article/details/gvmldyeka.sHtML

ANALYZE TABLE users;
来源：http://wap.hesvh.cn/Article/details/gqnhooksf.sHtML

[Q71] 查看建表语句
来源：http://blog.hesvh.cn/Article/details/gqjolithq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.hesvh.cn/Article/details/grrhelakg.sHtML

[Q72] 查看索引
来源：http://www.blog.fehbvm.com/Article/details/gbkevuemi.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/guxcozryx.sHtML

[Q73] 查看表状态
来源：http://blog.fehbvm.com/Article/details/ghmgueecl.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.zdbjq.cn/Article/details/ghegvbiig.sHtML

[Q74] 强制使用索引
来源：http://mobile.fehbvm.com/Article/details/gzuhzgxyj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.hesvh.cn/Article/details/gqtfxzelu.sHtML

[Q75] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gisufhowl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gqqhnslst.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.hesvh.cn/Article/details/gpobhrfkz.sHtML

[Q76] 按天统计
来源：http://www.m.share.hesvh.cn/Article/details/gscwpwidi.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.hesvh.cn/Article/details/glqebeeoj.sHtML

[Q77] 时间加减
来源：http://read.share.fehbvm.com/Article/details/guctwmihw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fehbvm.com/Article/details/gonkrzbwi.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/gzfogayxx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fehbvm.com/Article/details/gdakqiwiv.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gfphhbpef.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.zdbjq.cn/Article/details/gxvrejmcr.sHtML

[Q80] 字符串截取
来源：http://blog.fehbvm.com/Article/details/grvzcgqvs.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gphcqsvws.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gmyikkvgo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.hesvh.cn/Article/details/ggpkltnht.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/gezozcfal.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gixxjhjxf.sHtML

[Q83] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gjoqxvmoq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gwwddhwpc.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fehbvm.com/Article/details/gcbfowyba.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gupnmrdum.sHtML

[Q85] 数值取整
来源：http://mobile.fehbvm.com/Article/details/gydurkxfh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.hesvh.cn/Article/details/gwlynffsv.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.hesvh.cn/Article/details/gvadnojuo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.zdbjq.cn/Article/details/gjhhpysrb.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.zdbjq.cn/Article/details/gkwcwkktc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.hesvh.cn/Article/details/gpmioluef.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.zdbjq.cn/Article/details/ghiqeytjc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.hesvh.cn/Article/details/gkihgsyeq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.hesvh.cn/Article/details/gflscndrs.sHtML

[Q89] 判断表是否存在
来源：http://mobile.zdbjq.cn/Article/details/gahtwesww.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fehbvm.com/Article/details/godrdisuu.sHtML

[Q90] 生成序号列
来源：http://baike.zdbjq.cn/Article/details/gxxzfxfuf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.zdbjq.cn/Article/details/gonmizkds.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gzulrkcvl.sHtML

R. Bash 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gsapaqesb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gbujtxpqg.sHtML

[R01] shebang 与严格模式
来源：http://wap.fehbvm.com/Article/details/goykhnqyc.sHtML

#!/usr/bin/env bash
来源：http://baike.hesvh.cn/Article/details/gyvxdvcon.sHtML

set -euo pipefail
来源：http://m.share.zdbjq.cn/Article/details/gkywdjjqz.sHtML

[R02] 变量赋值与使用
来源：http://wap.fehbvm.com/Article/details/gwqwtngbc.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.hesvh.cn/Article/details/gxpjzbhxj.sHtML

[R03] 只读变量
来源：http://m.share.zdbjq.cn/Article/details/gjgwhvvrq.sHtML

readonly PI=3.14
来源：http://3g.fehbvm.com/Article/details/ggftyrvgi.sHtML

[R04] 位置参数
来源：http://mobile.fehbvm.com/Article/details/gginuvotl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.zdbjq.cn/Article/details/gcxvlahfo.sHtML

[R05] 参数默认值
来源：http://wap.fehbvm.com/Article/details/gycugomit.sHtML

name="${1:-default}"
来源：http://www.m.share.zdbjq.cn/Article/details/glcecaids.sHtML

[R06] 判断命令是否存在
来源：http://blog.hesvh.cn/Article/details/gdxdasatg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gghtojzry.sHtML

[R07] if 判断文件
来源：http://baike.zdbjq.cn/Article/details/gnfxlivrj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.zdbjq.cn/Article/details/gkcnlbooq.sHtML

[R08] 数值比较
来源：http://m.share.fehbvm.com/Article/details/gntqfqbyr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.hesvh.cn/Article/details/goafyljmu.sHtML

[R09] 字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gaarimqxx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/gcjzfibsi.sHtML

[R10] 正则匹配
来源：http://read.share.fehbvm.com/Article/details/gypljsvev.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.zdbjq.cn/Article/details/goyejdftm.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/gonvoioyo.sHtML

case "$1" in
来源：http://mobile.fehbvm.com/Article/details/gotkocvri.sHtML

start) echo "启动" ;;
来源：http://3g.fehbvm.com/Article/details/ghjdsaahh.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fehbvm.com/Article/details/gcloijezr.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/gjxakpxhf.sHtML

esac
来源：http://www.share.hesvh.cn/Article/details/grfgzdrwc.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/gsttfoqwc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.hesvh.cn/Article/details/gsskruluc.sHtML

[R13] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/giffbpsqb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gmfhudelf.sHtML

[R14] C 风格 for
来源：http://www.m.share.hesvh.cn/Article/details/ghumchscq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/grhwuaewt.sHtML

[R15] while 逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gmuckhyqs.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fehbvm.com/Article/details/gxgtukupi.sHtML

[R16] until 等待条件
来源：http://mobile.fehbvm.com/Article/details/gjnnjaxwe.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gueljiinh.sHtML

[R17] 数组定义与取值
来源：http://blog.hesvh.cn/Article/details/ghweqgzfv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gmewofaef.sHtML

[R18] 遍历数组
来源：http://read.share.hesvh.cn/Article/details/glcscrylq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.zdbjq.cn/Article/details/gveufdpyf.sHtML

[R19] 数组长度
来源：http://wap.fehbvm.com/Article/details/gkmrmxlvj.sHtML

echo "${#arr[@]}"
来源：http://read.share.hesvh.cn/Article/details/gjhlkxrcn.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fehbvm.com/Article/details/gkeoxqrqt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fehbvm.com/Article/details/gxugkhbki.sHtML

[R21] 字符串长度
来源：http://3g.zdbjq.cn/Article/details/gsyltiouw.sHtML

echo "${#s}"
来源：http://blog.hesvh.cn/Article/details/gptthntyv.sHtML

[R22] 截取子串
来源：http://wap.zdbjq.cn/Article/details/glcmdfonw.sHtML

echo "${s:0:5}"
来源：http://www.blog.zdbjq.cn/Article/details/gctigmkjk.sHtML

[R23] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gxvfphrcb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.hesvh.cn/Article/details/gihaknhno.sHtML

[R24] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gdiilixlt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.hesvh.cn/Article/details/gqlxwjzcx.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.zdbjq.cn/Article/details/gcnoxzysh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.hesvh.cn/Article/details/grytsmvsl.sHtML

[R26] 命令替换
来源：http://www.m.share.fehbvm.com/Article/details/guytswibp.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/gnuvdxusw.sHtML

[R27] 算术展开
来源：http://blog.zdbjq.cn/Article/details/gsoduxlyd.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fehbvm.com/Article/details/gklhechyt.sHtML

[R28] 浮点运算
来源：http://read.share.zdbjq.cn/Article/details/ghtcyvcqa.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.hesvh.cn/Article/details/grjzzbxih.sHtML

[R29] 定义函数
来源：http://m.share.zdbjq.cn/Article/details/gsrvtndki.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fehbvm.com/Article/details/gwqssjjnz.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fehbvm.com/Article/details/gjxhewdcp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/gkagtsehv.sHtML

[R31] 局部变量
来源：http://blog.fehbvm.com/Article/details/ghasvzrqn.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fehbvm.com/Article/details/gysakguxm.sHtML

[R32] 参数个数校验
来源：http://3g.fehbvm.com/Article/details/gxizhetdz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gpqkspwgn.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fehbvm.com/Article/details/gljhwrnjc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/gjnaeapbq.sHtML

[R34] 退出时清理
来源：http://www.m.share.zdbjq.cn/Article/details/gfzsqryjr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gneuehqix.sHtML

[R35] 后台执行并等待
来源：http://mobile.zdbjq.cn/Article/details/gnclaqfmy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.zdbjq.cn/Article/details/goeumhxrw.sHtML

[R36] 并发执行多个任务
来源：http://blog.hesvh.cn/Article/details/giynqdtwf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fehbvm.com/Article/details/galolhvjt.sHtML

[R37] 把输出赋给变量
来源：http://read.share.zdbjq.cn/Article/details/glxereotb.sHtML

files=$(ls -1)
来源：http://3g.hesvh.cn/Article/details/gbsbffbdq.sHtML

[R38] 管道串联
来源：http://www.m.share.zdbjq.cn/Article/details/gvcwrlcay.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.zdbjq.cn/Article/details/gjzeqikae.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fehbvm.com/Article/details/gsctyxnfq.sHtML

cmd > out.log 2>&1
来源：http://baike.zdbjq.cn/Article/details/gswnhsszg.sHtML

[R40] 追加写日志
来源：http://mobile.fehbvm.com/Article/details/gvyqexgfp.sHtML

echo "log" >> out.log
来源：http://read.share.zdbjq.cn/Article/details/gpocqxjee.sHtML

[R41] 丢弃输出
来源：http://read.share.zdbjq.cn/Article/details/giyqjqdqk.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.hesvh.cn/Article/details/grmbajrwk.sHtML

[R42] 输入重定向
来源：http://blog.hesvh.cn/Article/details/gvfedxhcf.sHtML

wc -l < a.txt
来源：http://m.share.zdbjq.cn/Article/details/ghxlehxdi.sHtML

[R43] 按名字查找文件
来源：http://blog.fehbvm.com/Article/details/gxmstxkkv.sHtML

find . -name "*.log" -type f
来源：http://mobile.hesvh.cn/Article/details/guxatqflr.sHtML

[R44] 按修改时间查找
来源：http://m.share.zdbjq.cn/Article/details/gshmszmel.sHtML

find . -mtime -7 -type f
来源：http://blog.fehbvm.com/Article/details/gpwygdort.sHtML

[R45] 批量删除
来源：http://read.share.fehbvm.com/Article/details/gchokkinq.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.hesvh.cn/Article/details/gwmvpgmbd.sHtML

[R46] 递归替换文件内容
来源：http://3g.zdbjq.cn/Article/details/gfbgbyoqv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/ghtdtqhox.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/gknsfpfll.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fehbvm.com/Article/details/gsgsuhnrc.sHtML

[R48] awk 取指定列
来源：http://www.share.hesvh.cn/Article/details/goztawvur.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fehbvm.com/Article/details/gptkenxqj.sHtML

[R49] awk 带条件
来源：http://wap.fehbvm.com/Article/details/gpeeekfox.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.zdbjq.cn/Article/details/gmwuyymox.sHtML

[R50] awk 求和
来源：http://3g.hesvh.cn/Article/details/gyjcqvmcd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/ghojlacup.sHtML

[R51] 排序去重取前几
来源：http://www.share.fehbvm.com/Article/details/gekvophia.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/gbafebsmx.sHtML

[R52] 统计行数
来源：http://m.share.fehbvm.com/Article/details/grnvhudsg.sHtML

wc -l a.txt
来源：http://m.share.zdbjq.cn/Article/details/gchzgssjl.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fehbvm.com/Article/details/goxbpobov.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.zdbjq.cn/Article/details/glbrslgwc.sHtML

[R54] 比较两个文件
来源：http://www.share.fehbvm.com/Article/details/gqjvgzubq.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/gbihrwxse.sHtML

[R55] 压缩与解压
来源：http://wap.fehbvm.com/Article/details/gnslkqahc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.hesvh.cn/Article/details/goohqsvok.sHtML

[R56] 远程拷贝
来源：http://m.share.hesvh.cn/Article/details/gvezsqrzh.sHtML

scp file user@host:/path/
来源：http://m.share.zdbjq.cn/Article/details/gxglmnyfj.sHtML

[R57] 远程执行命令
来源：http://www.share.hesvh.cn/Article/details/gbcixmhok.sHtML

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/grgsbviwj.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/gzehfzqqm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.zdbjq.cn/Article/details/gzyjrmrjl.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gzkolevub.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fehbvm.com/Article/details/gxoubjpsm.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gbjlzrggm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fehbvm.com/Article/details/grsywuhow.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/gontkzhej.sHtML

df -h;  du -sh *
来源：http://read.share.hesvh.cn/Article/details/gmmqizqdb.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.hesvh.cn/Article/details/gcholpcqk.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/gchnqlflw.sHtML

[R63] 内存与进程
来源：http://blog.zdbjq.cn/Article/details/gyubrtybp.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.hesvh.cn/Article/details/gewjxlrqb.sHtML

[R64] 结束进程
来源：http://blog.fehbvm.com/Article/details/gvbkglwgl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fehbvm.com/Article/details/gomjteznq.sHtML

[R65] 查看端口占用
来源：http://blog.hesvh.cn/Article/details/gwjzardgp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.zdbjq.cn/Article/details/gieuilwax.sHtML

[R66] 定时任务
来源：http://baike.fehbvm.com/Article/details/ggicttdrv.sHtML

crontab -e;  crontab -l
来源：http://baike.hesvh.cn/Article/details/gzggdkyjm.sHtML

[R67] 生成随机十六进制串
来源：http://blog.zdbjq.cn/Article/details/gworpkotk.sHtML

openssl rand -hex 16
来源：http://mobile.hesvh.cn/Article/details/gaaneawit.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/gjnxeblic.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/gcjklgwkv.sHtML

[R69] 生成随机密码
来源：http://3g.fehbvm.com/Article/details/ggzdndsms.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/guoxmoarc.sHtML

[R70] 时间戳与互转
来源：http://m.share.zdbjq.cn/Article/details/gxiihizjd.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.zdbjq.cn/Article/details/gofgvfhyp.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gfqlfwzpj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fehbvm.com/Article/details/gfripohlq.sHtML

[R72] 等待端口就绪
来源：http://3g.fehbvm.com/Article/details/gnkotjila.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gwinxciyl.sHtML

[R73] 分割大日志
来源：http://3g.hesvh.cn/Article/details/gvhqygbek.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/gczohdynf.sHtML

[R74] 批量重命名
来源：http://mobile.zdbjq.cn/Article/details/gxchhqiiy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.hesvh.cn/Article/details/gxwdtytab.sHtML

[R75] 导出环境变量
来源：http://www.blog.hesvh.cn/Article/details/gixgnodwq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.hesvh.cn/Article/details/gjnrjdvmn.sHtML

[R76] 使用临时文件
来源：http://www.share.zdbjq.cn/Article/details/gpjfxlrzx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gdpisbjir.sHtML

[R77] 读取用户输入
来源：http://3g.hesvh.cn/Article/details/gxlqchlec.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/gkfzwblvn.sHtML

[R78] 交互式菜单
来源：http://www.blog.fehbvm.com/Article/details/gkywvoica.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.hesvh.cn/Article/details/gplbwzoja.sHtML

[R79] 解析命令行选项
来源：http://wap.hesvh.cn/Article/details/gmceyrxcp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.hesvh.cn/Article/details/gopryopkz.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fehbvm.com/Article/details/guhakzkxp.sHtML

time ./run.sh
来源：http://mobile.fehbvm.com/Article/details/gfjwcbznk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gygvetlsl.sHtML

S. C / C++ 专题
来源：http://www.share.zdbjq.cn/Article/details/ghmiseawa.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gpraowhwq.sHtML

[S01] C：Hello World
来源：http://blog.hesvh.cn/Article/details/gbmvumkfl.sHtML

#include <stdio.h>
来源：http://m.share.zdbjq.cn/Article/details/gqmksmeet.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.hesvh.cn/Article/details/gjtnbrdhn.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fehbvm.com/Article/details/ghlvadojk.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/gnymliiok.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/geyufmqed.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.hesvh.cn/Article/details/geomglcvm.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/gmabukcmv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/grzuvebvm.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/gqzivfecd.sHtML

strlen(s)
来源：http://m.share.fehbvm.com/Article/details/gwpogrzcs.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/gtvmbzcsl.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.hesvh.cn/Article/details/gxypfxvvz.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/gsjkpqtar.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.hesvh.cn/Article/details/ghtxrvsif.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fehbvm.com/Article/details/gmlxofard.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fehbvm.com/Article/details/gurikotfk.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.zdbjq.cn/Article/details/gyzhdrqrx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fehbvm.com/Article/details/gspijciew.sHtML

[S10] C：指针与解引用
来源：http://m.share.hesvh.cn/Article/details/gdfyzoddv.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fehbvm.com/Article/details/gpvogxovu.sHtML

[S11] C：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gpjgroils.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/gnuvzqjad.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/gxvezgpzq.sHtML

fclose(f);
来源：http://wap.hesvh.cn/Article/details/gzsknoevj.sHtML

[S12] C：写文件
来源：http://baike.fehbvm.com/Article/details/gwfxfumoz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gutrjjucq.sHtML

[S13] C：宏定义
来源：http://baike.hesvh.cn/Article/details/gmiooqvhp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fehbvm.com/Article/details/gxernjqrr.sHtML

[S14] C：枚举
来源：http://wap.zdbjq.cn/Article/details/grbbxtjou.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/gsstnrqvp.sHtML

[S15] C：类型转换
来源：http://m.share.zdbjq.cn/Article/details/gpmltkbbt.sHtML

(double) a / b
来源：http://www.m.share.fehbvm.com/Article/details/gyqdyljew.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/guxbvvjnb.sHtML

x |= (1 << 3);
来源：http://baike.fehbvm.com/Article/details/gxswjzmno.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.hesvh.cn/Article/details/guesfciak.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/gcafnaehr.sHtML

[S18] C：命令行参数
来源：http://www.share.fehbvm.com/Article/details/gzjwisuyt.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fehbvm.com/Article/details/gxfuhljet.sHtML

[S19] C：快速排序
来源：http://baike.zdbjq.cn/Article/details/ghuzpdfrp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gjyexlmgv.sHtML

[S20] C：二分查找
来源：http://wap.fehbvm.com/Article/details/gyooqjmzc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gcaihjted.sHtML

[S21] C：字符类别判断
来源：http://www.share.hesvh.cn/Article/details/gtedsesrs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.zdbjq.cn/Article/details/gxsxbmdhk.sHtML

[S22] C：字符串转数字
来源：http://wap.fehbvm.com/Article/details/gaycfybel.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.hesvh.cn/Article/details/gwfeusjbk.sHtML

[S23] C：随机数
来源：http://www.blog.zdbjq.cn/Article/details/gpatuvddh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/geddrrqyk.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/gpzohehsz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.hesvh.cn/Article/details/gztdyvrcj.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/gtcpvybjs.sHtML

memcpy(dst, src, n);
来源：http://www.share.zdbjq.cn/Article/details/gfqjtbxyg.sHtML

[S26] C：内存清零
来源：http://3g.hesvh.cn/Article/details/gqhfsonrz.sHtML

memset(a, 0, sizeof a);
来源：http://wap.hesvh.cn/Article/details/gciiyvbpk.sHtML

[S27] C：定义常量
来源：http://m.share.zdbjq.cn/Article/details/gsruknnkw.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gzhfwspnf.sHtML

[S28] C：静态变量
来源：http://blog.hesvh.cn/Article/details/gwnnausvg.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/gkbexksit.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/gdizrnzly.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/geoummeqm.sHtML

[S30] C：头文件保护
来源：http://read.share.hesvh.cn/Article/details/gdkbyeopj.sHtML

#ifndef X_H
来源：http://wap.fehbvm.com/Article/details/ghchdxexj.sHtML

#define X_H
来源：http://wap.fehbvm.com/Article/details/ghcqmupmo.sHtML

#endif
来源：http://www.m.share.hesvh.cn/Article/details/gcrsnhhkg.sHtML

[S31] C++：Hello World
来源：http://baike.fehbvm.com/Article/details/guqduipzq.sHtML

#include <iostream>
来源：http://wap.hesvh.cn/Article/details/gxjgtwgtg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gurlmdyqz.sHtML

[S32] C++：字符串
来源：http://www.blog.fehbvm.com/Article/details/gfonjkqay.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.hesvh.cn/Article/details/gyomgbocm.sHtML

[S33] C++：vector 增删
来源：http://wap.hesvh.cn/Article/details/grcsrcufa.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/grsnzygst.sHtML

[S34] C++：遍历 vector
来源：http://3g.zdbjq.cn/Article/details/gwvtyvzao.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/gqxeyzano.sHtML


<!-- 参考信息 -->