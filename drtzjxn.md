代发 wailian999

[Q67] 设置隔离级别
来源：http://www.share.zdbjq.cn/Article/details/gybgvlzls.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.hesvh.cn/Article/details/gqbhywbps.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/gcjxpqrlp.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gbzylbtnl.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fehbvm.com/Article/details/gfkialoon.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/giwrfdsiv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.hesvh.cn/Article/details/gghcbkxye.sHtML

[Q70] 更新统计信息
来源：http://m.share.zdbjq.cn/Article/details/gupqjvlqs.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fehbvm.com/Article/details/gigilyfaa.sHtML

[Q71] 查看建表语句
来源：http://www.blog.zdbjq.cn/Article/details/gdpjzmled.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fehbvm.com/Article/details/gmboyxpqb.sHtML

[Q72] 查看索引
来源：http://m.share.zdbjq.cn/Article/details/geusiypzk.sHtML

SHOW INDEX FROM users;
来源：http://3g.fehbvm.com/Article/details/gwfbizzoz.sHtML

[Q73] 查看表状态
来源：http://baike.zdbjq.cn/Article/details/grvxzgakv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.zdbjq.cn/Article/details/gzhfsstft.sHtML

[Q74] 强制使用索引
来源：http://baike.zdbjq.cn/Article/details/giszoexxm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.zdbjq.cn/Article/details/gprsvrdxf.sHtML

[Q75] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gakhfabwh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gafqdxevb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.hesvh.cn/Article/details/gbzqqmmhe.sHtML

[Q76] 按天统计
来源：http://www.blog.hesvh.cn/Article/details/gnsmagedl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fehbvm.com/Article/details/grkxzlicl.sHtML

[Q77] 时间加减
来源：http://mobile.hesvh.cn/Article/details/gzbtvtlxp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fehbvm.com/Article/details/gfhebyhfm.sHtML

[Q78] 当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gkwmcqowg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fehbvm.com/Article/details/gqbnvyhqt.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gvirveuky.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fehbvm.com/Article/details/gvcppxzmn.sHtML

[Q80] 字符串截取
来源：http://mobile.fehbvm.com/Article/details/gjcyudguk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gtisnjeom.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gbcxggpld.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.zdbjq.cn/Article/details/gspfyjyvk.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/grhdmcbbi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/guufdujbq.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/galijezqt.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gzpnwrzph.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.hesvh.cn/Article/details/gqkmbcpml.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/glotwmstr.sHtML

[Q85] 数值取整
来源：http://www.m.share.fehbvm.com/Article/details/gulqgxhtr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fehbvm.com/Article/details/gsljyrzdh.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.zdbjq.cn/Article/details/giecyvjqm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fehbvm.com/Article/details/ghokozenm.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.zdbjq.cn/Article/details/gurfbdsab.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.zdbjq.cn/Article/details/gdhohowen.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.zdbjq.cn/Article/details/ghjmlurip.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.hesvh.cn/Article/details/gfyxqvpfk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/gwcxvqrfb.sHtML

[Q89] 判断表是否存在
来源：http://baike.zdbjq.cn/Article/details/godapqecu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fehbvm.com/Article/details/gueuucqaa.sHtML

[Q90] 生成序号列
来源：http://www.blog.hesvh.cn/Article/details/gkvhfxiix.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/gsbgpztiq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gsujrzrlx.sHtML

R. Bash 专题
来源：http://read.share.zdbjq.cn/Article/details/gduxqfbtx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gljbayifu.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fehbvm.com/Article/details/gscafpmvw.sHtML

#!/usr/bin/env bash
来源：http://m.share.fehbvm.com/Article/details/gczxdwehd.sHtML

set -euo pipefail
来源：http://baike.fehbvm.com/Article/details/gwvdxuojr.sHtML

[R02] 变量赋值与使用
来源：http://blog.fehbvm.com/Article/details/gdqnbnanf.sHtML

name="Tom"; echo "$name"
来源：http://wap.zdbjq.cn/Article/details/gznzunutg.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/gjhhtdpzu.sHtML

readonly PI=3.14
来源：http://wap.hesvh.cn/Article/details/gcndpgfyz.sHtML

[R04] 位置参数
来源：http://3g.fehbvm.com/Article/details/gxdvpwpuf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.hesvh.cn/Article/details/gzzcigrpb.sHtML

[R05] 参数默认值
来源：http://read.share.hesvh.cn/Article/details/ghscksqrd.sHtML

name="${1:-default}"
来源：http://mobile.fehbvm.com/Article/details/gjwbpupfr.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gwjvqoqvw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gpgjjncer.sHtML

[R07] if 判断文件
来源：http://read.share.zdbjq.cn/Article/details/gczfkvjsr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.zdbjq.cn/Article/details/gyzbrjqhb.sHtML

[R08] 数值比较
来源：http://baike.hesvh.cn/Article/details/gwplmxwtp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.zdbjq.cn/Article/details/gohoenhmq.sHtML

[R09] 字符串比较
来源：http://blog.fehbvm.com/Article/details/gsuctfeok.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.zdbjq.cn/Article/details/galtqpexo.sHtML

[R10] 正则匹配
来源：http://wap.hesvh.cn/Article/details/gmazhpxht.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fehbvm.com/Article/details/gsgnszsxw.sHtML

[R11] case 多分支
来源：http://wap.fehbvm.com/Article/details/gcznzitxf.sHtML

case "$1" in
来源：http://m.share.hesvh.cn/Article/details/gzjqmutfz.sHtML

start) echo "启动" ;;
来源：http://mobile.zdbjq.cn/Article/details/glkoplmix.sHtML

stop)  echo "停止" ;;
来源：http://m.share.zdbjq.cn/Article/details/gmxumjedq.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/gxomjciti.sHtML

esac
来源：http://www.blog.fehbvm.com/Article/details/gsnzivqpp.sHtML

[R12] for 遍历文件
来源：http://wap.fehbvm.com/Article/details/gejuecivh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/gvfqgcbbm.sHtML

[R13] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/gvrhpblbb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gykiokdrc.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/gurikdxhg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gzkxwsrig.sHtML

[R15] while 逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gzxzlrmuz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.hesvh.cn/Article/details/gisbosoxg.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/gqysljcwa.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gavhjfsct.sHtML

[R17] 数组定义与取值
来源：http://m.share.fehbvm.com/Article/details/gtengdhxi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/gyvclkavj.sHtML

[R18] 遍历数组
来源：http://www.blog.fehbvm.com/Article/details/gmdnvudcb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.hesvh.cn/Article/details/gcyuwexii.sHtML

[R19] 数组长度
来源：http://baike.fehbvm.com/Article/details/goxwnpzun.sHtML

echo "${#arr[@]}"
来源：http://www.blog.hesvh.cn/Article/details/gpykxqivv.sHtML

[R20] 关联数组（字典）
来源：http://wap.fehbvm.com/Article/details/gfvxiblkg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.hesvh.cn/Article/details/gjupfance.sHtML

[R21] 字符串长度
来源：http://read.share.hesvh.cn/Article/details/gpcrcijms.sHtML

echo "${#s}"
来源：http://read.share.hesvh.cn/Article/details/grhjamizy.sHtML

[R22] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gjzdzwinj.sHtML

echo "${s:0:5}"
来源：http://blog.hesvh.cn/Article/details/ghfiwfdzt.sHtML

[R23] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gwjblpidz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/gfentmyas.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/ggndtfzhx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.zdbjq.cn/Article/details/gadbnpnfe.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fehbvm.com/Article/details/gcdtrpldz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.hesvh.cn/Article/details/gtvovwpnn.sHtML

[R26] 命令替换
来源：http://www.blog.zdbjq.cn/Article/details/gktiwsorw.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.zdbjq.cn/Article/details/gcepspqbj.sHtML

[R27] 算术展开
来源：http://3g.zdbjq.cn/Article/details/gyegstpjd.sHtML

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/gdlwtlabq.sHtML

[R28] 浮点运算
来源：http://3g.zdbjq.cn/Article/details/grzahqrbu.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.zdbjq.cn/Article/details/gqllixxcl.sHtML

[R29] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gurvwhrul.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/gyskhijlh.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/gxntlwcth.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/gdbmqydue.sHtML

[R31] 局部变量
来源：http://m.share.hesvh.cn/Article/details/gfmrnvpnh.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.hesvh.cn/Article/details/gkxwxdekb.sHtML

[R32] 参数个数校验
来源：http://www.share.fehbvm.com/Article/details/ggcvnkpow.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gyeapzkml.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/gixyztlwz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/gytmggmgo.sHtML

[R34] 退出时清理
来源：http://www.share.zdbjq.cn/Article/details/gwomgwzir.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/ghbykpoph.sHtML

[R35] 后台执行并等待
来源：http://www.share.fehbvm.com/Article/details/ggobzesvs.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fehbvm.com/Article/details/gzchtrjiz.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.hesvh.cn/Article/details/gxcwqnvqw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.hesvh.cn/Article/details/gtjjyjduj.sHtML

[R37] 把输出赋给变量
来源：http://read.share.zdbjq.cn/Article/details/gizuaitgv.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/gdbxzgmqc.sHtML

[R38] 管道串联
来源：http://wap.zdbjq.cn/Article/details/gflbdlriy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.hesvh.cn/Article/details/gmowkjcln.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fehbvm.com/Article/details/ggogehpoh.sHtML

cmd > out.log 2>&1
来源：http://baike.hesvh.cn/Article/details/gmuxchfmw.sHtML

[R40] 追加写日志
来源：http://mobile.fehbvm.com/Article/details/gsfjabuvo.sHtML

echo "log" >> out.log
来源：http://www.share.zdbjq.cn/Article/details/gdooxfgit.sHtML

[R41] 丢弃输出
来源：http://www.share.zdbjq.cn/Article/details/gepjlqpxn.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gfbtfmxgh.sHtML

[R42] 输入重定向
来源：http://read.share.fehbvm.com/Article/details/gcztvrsdn.sHtML

wc -l < a.txt
来源：http://mobile.hesvh.cn/Article/details/gglyyefhc.sHtML

[R43] 按名字查找文件
来源：http://blog.hesvh.cn/Article/details/gtijniczp.sHtML

find . -name "*.log" -type f
来源：http://wap.hesvh.cn/Article/details/glzqblolh.sHtML

[R44] 按修改时间查找
来源：http://www.share.fehbvm.com/Article/details/gnopcpysq.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gjitazkcv.sHtML

[R45] 批量删除
来源：http://baike.hesvh.cn/Article/details/gxpthzdpd.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fehbvm.com/Article/details/gifhxjxcm.sHtML

[R46] 递归替换文件内容
来源：http://wap.zdbjq.cn/Article/details/gbrktgoup.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.hesvh.cn/Article/details/gwidrclyl.sHtML

[R47] sed 单行替换
来源：http://3g.zdbjq.cn/Article/details/gfmzzdtnx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gfczqanjr.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/gvxuyexdp.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gevwatlzh.sHtML

[R49] awk 带条件
来源：http://wap.fehbvm.com/Article/details/grxrptpcg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fehbvm.com/Article/details/gqphsycdk.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/gyhxubxew.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gwgyetkbn.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/gnogbofgf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.zdbjq.cn/Article/details/gtnhousay.sHtML

[R52] 统计行数
来源：http://3g.hesvh.cn/Article/details/gzciiluqg.sHtML

wc -l a.txt
来源：http://www.share.hesvh.cn/Article/details/gdltjiihh.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fehbvm.com/Article/details/gewydalcq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.zdbjq.cn/Article/details/gdcwyxeud.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/gyuihmarz.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/gfjoexcyo.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/grawkzjab.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fehbvm.com/Article/details/guldixlhn.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gfdztayjn.sHtML

scp file user@host:/path/
来源：http://blog.zdbjq.cn/Article/details/ghyfvqkry.sHtML

[R57] 远程执行命令
来源：http://read.share.hesvh.cn/Article/details/gjexktlse.sHtML

ssh user@host 'uptime'
来源：http://blog.hesvh.cn/Article/details/gdaudokwf.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/gtqidodgd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.zdbjq.cn/Article/details/gufqwbgug.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gqdzlgvcj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.hesvh.cn/Article/details/gydexxcvd.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gyfggqsyj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/gqmnvfrkj.sHtML

[R61] 磁盘占用
来源：http://m.share.fehbvm.com/Article/details/gnxusbysc.sHtML

df -h;  du -sh *
来源：http://baike.fehbvm.com/Article/details/gtwjfaelb.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.hesvh.cn/Article/details/gjxmwhqzr.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/gborppsnd.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/gmfnhpovw.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.hesvh.cn/Article/details/ghylxdapx.sHtML

[R64] 结束进程
来源：http://3g.hesvh.cn/Article/details/ghcrlspdl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.hesvh.cn/Article/details/gcwvrrjqe.sHtML

[R65] 查看端口占用
来源：http://mobile.hesvh.cn/Article/details/gjlxhwvot.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/ghfiikjbi.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/gikgsxmru.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/grkueqsvi.sHtML

[R67] 生成随机十六进制串
来源：http://baike.zdbjq.cn/Article/details/grxastosz.sHtML

openssl rand -hex 16
来源：http://baike.zdbjq.cn/Article/details/gjlpvzzqf.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/gprzarkdq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.hesvh.cn/Article/details/gptdzynht.sHtML

[R69] 生成随机密码
来源：http://mobile.fehbvm.com/Article/details/ghfwldybs.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.hesvh.cn/Article/details/gvxlhkgej.sHtML

[R70] 时间戳与互转
来源：http://baike.hesvh.cn/Article/details/gppfdjker.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fehbvm.com/Article/details/galjlaowu.sHtML

[R71] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gnzkpcmju.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/gudfeozbu.sHtML

[R72] 等待端口就绪
来源：http://baike.hesvh.cn/Article/details/gvpaxacpt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gekefmbbf.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/gobpmwtsl.sHtML

split -l 1000 big.log part_
来源：http://3g.fehbvm.com/Article/details/gwdszektu.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/gpnfzvwpg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/gqudysscm.sHtML

[R75] 导出环境变量
来源：http://blog.zdbjq.cn/Article/details/gypojkebh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.zdbjq.cn/Article/details/gtzbltnse.sHtML

[R76] 使用临时文件
来源：http://wap.hesvh.cn/Article/details/gjnpfwmlu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gjyhvxhmc.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/gnolykgki.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/guwwfzane.sHtML

[R78] 交互式菜单
来源：http://mobile.zdbjq.cn/Article/details/gwxijtqri.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.zdbjq.cn/Article/details/gsrelcgij.sHtML

[R79] 解析命令行选项
来源：http://read.share.fehbvm.com/Article/details/gomxtdzzo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.zdbjq.cn/Article/details/gxtcicxjk.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/gnobiyheo.sHtML

time ./run.sh
来源：http://baike.fehbvm.com/Article/details/ghmvsodtp.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbfszsuyx.sHtML

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/gafwmeseb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghcoxedbk.sHtML

[S01] C：Hello World
来源：http://wap.zdbjq.cn/Article/details/gvlobelpg.sHtML

#include <stdio.h>
来源：http://m.share.zdbjq.cn/Article/details/gogevoqzm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.zdbjq.cn/Article/details/gydfbnrmc.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fehbvm.com/Article/details/gqruefmlm.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fehbvm.com/Article/details/gcndbkqvj.sHtML

[S03] C：读入整数
来源：http://www.share.zdbjq.cn/Article/details/gwangjlva.sHtML

int x; scanf("%d", &x);
来源：http://wap.fehbvm.com/Article/details/gpyqoebyj.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/gxwgzjwkb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gredkvoeo.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/gievgmyzk.sHtML

strlen(s)
来源：http://read.share.zdbjq.cn/Article/details/gztdcqgme.sHtML

[S06] C：字符串比较
来源：http://read.share.fehbvm.com/Article/details/grhwacehh.sHtML

strcmp(a, b) == 0
来源：http://www.share.fehbvm.com/Article/details/gjibpugxn.sHtML

[S07] C：数组遍历求和
来源：http://3g.hesvh.cn/Article/details/gszjhsjzz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.zdbjq.cn/Article/details/gsnsyfscf.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/gvzcfepxs.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fehbvm.com/Article/details/gcjgxhufl.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.hesvh.cn/Article/details/gdroofpax.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fehbvm.com/Article/details/ggllyewqm.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/givdizqrw.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/gqolriysp.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/geqlgvssx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.zdbjq.cn/Article/details/geawmgonb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.hesvh.cn/Article/details/gmtwtwotz.sHtML

fclose(f);
来源：http://baike.hesvh.cn/Article/details/gmwdohejm.sHtML

[S12] C：写文件
来源：http://3g.fehbvm.com/Article/details/ghlpdzkpa.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fehbvm.com/Article/details/glqvplgqy.sHtML

[S13] C：宏定义
来源：http://m.share.fehbvm.com/Article/details/gtzjvaedg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.hesvh.cn/Article/details/gtqajgygx.sHtML

[S14] C：枚举
来源：http://mobile.zdbjq.cn/Article/details/gqbdjihde.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.hesvh.cn/Article/details/gummwyqzu.sHtML

[S15] C：类型转换
来源：http://m.share.hesvh.cn/Article/details/ggtltaxmc.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/gphdaulyp.sHtML

[S16] C：位操作置位
来源：http://m.share.hesvh.cn/Article/details/gvbksephy.sHtML

x |= (1 << 3);
来源：http://www.share.fehbvm.com/Article/details/gjdzhtmlo.sHtML

[S17] C：安全拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gfkbhfguy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fehbvm.com/Article/details/gawnidfcn.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/gdzgngokb.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fehbvm.com/Article/details/gfewkotoa.sHtML

[S19] C：快速排序
来源：http://read.share.hesvh.cn/Article/details/gvqevcgzr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gizxyinaa.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/gskgdmwyf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gnssoiyqq.sHtML

[S21] C：字符类别判断
来源：http://www.share.zdbjq.cn/Article/details/gcipvugzv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.hesvh.cn/Article/details/gkrzujiwr.sHtML

[S22] C：字符串转数字
来源：http://wap.hesvh.cn/Article/details/gbrbekqaz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.zdbjq.cn/Article/details/ghqmwldql.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/gqmtdbqgs.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/gdbblarhy.sHtML

[S24] C：获取本地时间
来源：http://m.share.fehbvm.com/Article/details/ghwonkpwv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.zdbjq.cn/Article/details/gyeeekiqe.sHtML

[S25] C：内存拷贝
来源：http://baike.hesvh.cn/Article/details/gnyntessy.sHtML

memcpy(dst, src, n);
来源：http://baike.zdbjq.cn/Article/details/geamfioax.sHtML

[S26] C：内存清零
来源：http://www.m.share.zdbjq.cn/Article/details/ghuxaybea.sHtML

memset(a, 0, sizeof a);
来源：http://wap.hesvh.cn/Article/details/gqliqlysk.sHtML

[S27] C：定义常量
来源：http://www.share.hesvh.cn/Article/details/gdyaahewy.sHtML

const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gbeohlghm.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/gkqcvgzih.sHtML

static int counter = 0;
来源：http://www.blog.fehbvm.com/Article/details/gksbqetxj.sHtML

[S29] C：变参函数
来源：http://wap.zdbjq.cn/Article/details/gzjljkwsk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fehbvm.com/Article/details/gpgzrxadu.sHtML

[S30] C：头文件保护
来源：http://m.share.zdbjq.cn/Article/details/gskuqmude.sHtML

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/gmsxxlmop.sHtML

#define X_H
来源：http://baike.zdbjq.cn/Article/details/gaxixxobg.sHtML

#endif
来源：http://wap.fehbvm.com/Article/details/gaynltbbt.sHtML

[S31] C++：Hello World
来源：http://blog.zdbjq.cn/Article/details/gscucfoti.sHtML

#include <iostream>
来源：http://baike.hesvh.cn/Article/details/grymbbudz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/gnzbteklf.sHtML

[S32] C++：字符串
来源：http://www.m.share.hesvh.cn/Article/details/gqdyzskik.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.zdbjq.cn/Article/details/gxslxccdt.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/gxajvdqxz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fehbvm.com/Article/details/gslwckmpx.sHtML

[S34] C++：遍历 vector
来源：http://mobile.zdbjq.cn/Article/details/gekxowezk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fehbvm.com/Article/details/gfdaqloac.sHtML

[S35] C++：map
来源：http://3g.hesvh.cn/Article/details/gdypxbbyi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gvbumchhb.sHtML

[S36] C++：unordered_map
来源：http://baike.zdbjq.cn/Article/details/grksmsbmf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/grsilkmjk.sHtML


<!-- 参考信息 -->