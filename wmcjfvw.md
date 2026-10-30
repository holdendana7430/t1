代发 wailian999

ROLLBACK TO sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/ggqmmebbr.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmsnglyfe.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fanxiaobao.xyz/Article/details/gyxcpwifg.sHtML

[Q70] 更新统计信息
来源：http://blog.fanxiaobao.xyz/Article/details/gfjzyujjx.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktwlahyq.sHtML

[Q71] 查看建表语句
来源：http://3g.fanxiaobao.xyz/Article/details/ghqnuptap.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fanxiaobao.xyz/Article/details/gjwxlhzdp.sHtML

[Q72] 查看索引
来源：http://www.share.fanxiaobao.xyz/Article/details/geuplaren.sHtML

SHOW INDEX FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gaptghkps.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpxbydfk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gzfdapdya.sHtML

[Q74] 强制使用索引
来源：http://baike.fanxiaobao.xyz/Article/details/gxblspzur.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fanxiaobao.xyz/Article/details/gnkcxumui.sHtML

[Q75] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gehgexngc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/grhseebbl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fanxiaobao.xyz/Article/details/gnbjqbfkr.sHtML

[Q76] 按天统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcriqloi.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/gnxbevcfp.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/grbvjwotm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitwgfhru.sHtML

[Q78] 当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhpwzdcg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fanxiaobao.xyz/Article/details/gydbdqwsm.sHtML

[Q79] 字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gscebnpfz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fanxiaobao.xyz/Article/details/gakvnxpvy.sHtML

[Q80] 字符串截取
来源：http://3g.fanxiaobao.xyz/Article/details/gncvazgqd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghabrdqme.sHtML

[Q81] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/grquzxqmz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggyxscoer.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fanxiaobao.xyz/Article/details/gmxvhfjtw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gvnurcvwh.sHtML

[Q83] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/guzphtrjc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfsvnpnx.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxclgyyoq.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gamrfnhyh.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/giyvqgxev.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fanxiaobao.xyz/Article/details/gecwdyann.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gluhijztv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fanxiaobao.xyz/Article/details/gluotluks.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fanxiaobao.xyz/Article/details/ghhviiokf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/gymtdfgwq.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvoyyyri.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqtdqevd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvumadhx.sHtML

[Q89] 判断表是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gpvudywos.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gbqtjiqrg.sHtML

[Q90] 生成序号列
来源：http://read.share.fanxiaobao.xyz/Article/details/gzueqzlem.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fanxiaobao.xyz/Article/details/giseemwmj.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gupnjanvk.sHtML

R. Bash 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gswqkfwhs.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjulvycyy.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhfnactl.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/glslfdxdj.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/gpbolsvwk.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsczpdic.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjncautsf.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/gsniipaba.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxyvhospn.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gawkyxusm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/gdsywinfu.sHtML

[R05] 参数默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gfnajaijt.sHtML

name="${1:-default}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxmysamj.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/ggojggikh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbhiagre.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/gnhfwmito.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gvdjsjcod.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwambmlo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbpmbjey.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gihirlxea.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gyxrvhoim.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gdghmhuvb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmgmxeec.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcjaxlgf.sHtML

case "$1" in
来源：http://baike.fanxiaobao.xyz/Article/details/garnbgdhj.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrrhdmpf.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbvjtocg.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtahoqftt.sHtML

esac
来源：http://www.share.fanxiaobao.xyz/Article/details/geveilyhi.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcnkqdpv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfrsnikd.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gvemckvjt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/groufjmso.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcpqnpsl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/grzwzyfex.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gvwestqjy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gowwclhjf.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/ggkqbpwmj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbsqlmlsg.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/gabnzzumy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvjkreur.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/gpqusibhu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykdjixfu.sHtML

[R19] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/gphuipcub.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyyajbvv.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhyykvaj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlkquuey.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gzhwganhm.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gclnzclqe.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gydqcjnka.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdijbjpt.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqewbxcj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gncbggtmk.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnfcjenq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gjmjhwlsn.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gusoywcvb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/geedyolja.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/giacgrqsp.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gosdkooyp.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrrzlgky.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/giwakedpo.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gzivaeuyr.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/gitvxkhyi.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxavbfgv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnnhscjq.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gxwqtreoz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/giaichucx.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbplasov.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gmauisfoi.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnroigjb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvogvsvte.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlrqypwf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/gjktqlcti.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/gbjqezhwn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gezqlvupy.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/ghlzanpae.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwlblhxt.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/glnsgtxze.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/gslwggdia.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgaoxpha.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlxazjjp.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbktysvm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gmklqiuke.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gskltaqrr.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gssppekrg.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbnejvtr.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gkeuelizh.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gddhzopyw.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/guqkbuxkf.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmunjiuf.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfyocelb.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzbahpmy.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyvfqmsj.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gnvlojjrr.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqwqkrul.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gdotqvjfz.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsciykbfu.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvjhbyui.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdldohql.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtdlustp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/glufgvlql.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbobovcj.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdoimrgg.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gzxawnvfx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkhtszwo.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfeydxkk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gtmukqjwj.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmulbpmt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/gztufjcxt.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gkwjzywkm.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gffydcamy.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/gwngyqrvz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/gbuuxrjxj.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdaveqdy.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/giypftcsy.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gkndqaamm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndmwterj.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhxleqhx.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrehfqku.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/guqgfskir.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzmydeje.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcnorfha.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdiakxwey.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozfvtlco.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbeciattw.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gufwxcwbt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gisvrfpva.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gdpcguxjv.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gsziseoxd.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/gfxnmxntq.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdadcbkb.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gqszpzeix.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gnyvwrvcc.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/guiwltuii.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/ggdsvqwfv.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gaiwxdnps.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/ghowyswka.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfxvecpj.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/geisofxiy.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwgdokxz.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/gtohfkoyh.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/giwyzylzx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvufbahe.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwiiyjuk.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geaepgnxo.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjpyqnqm.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gufluvubi.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gohkdalnj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/gpasxzycx.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gsudwnpgg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gtsumphye.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/ghteisgvr.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gvmaumpfa.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gsodkescc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gapvuchvm.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/ghskzsveq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgzgofte.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gpgoanqgc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvhmeqzj.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/goeinmceq.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/gaillrpjz.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/grkwhlkiq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/grhilzdmj.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gwxhfowhy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gkxdnzkli.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkbwsrvn.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/gkylzcgyg.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbqnwthy.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/ghfoomgpt.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gsjlrvydm.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gvhzodbmf.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/ghxcvnhhy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvtkvqyg.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/ghthpsfsf.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxedpqgka.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqmjoqln.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gbcgfgind.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gfutpvcjx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpqvvtrw.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gcklszytx.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlpncihd.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gcsvqiisi.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gddypoxzl.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gbtbzayuk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnrhutug.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewmurlgi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlikkshq.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/gpgryibzy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/guoasfzpm.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrcdwkcn.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/grunbfden.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgibbdyx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbkhwbdw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/goriouxva.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgzicsdo.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gpshbdqod.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gteidobfb.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gazteeobu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/glrrrqlle.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gaurcrpqy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gwbihfoiq.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwejrvsn.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmhkcxpp.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/gtucsscew.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbwlyeio.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxitlpsz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gffpskzkz.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpowzwni.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gqbldbvky.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/ggmqozzrg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gigfnjbbd.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gvszbpyqu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gxrndmepk.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftzkqzqy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbkweolz.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthwdtfkk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/gsznirzug.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gjtywolpj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gupfnkwbi.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gutqxizkz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gsjjtqjra.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gaabxslrm.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gcuhlxfpo.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkrrlopj.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtmcanhr.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/gqsomvvfd.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcddnpdpa.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/gatnsebox.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gxtemainm.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgampjdt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gewlevrsk.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmuslflhf.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gihgtlekx.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyhjjqmk.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gugnxfglg.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjvuhoht.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gpmnfddzp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjvhdvqs.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gxsahubfl.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/gimafujrb.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gaiodulcz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzpszvmx.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmbymjov.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyyrsatpl.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gdaprzinf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gehacogny.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqimhssjt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gggqjklzg.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxzgvyxu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejwfxtzj.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gmyylbofo.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gbycvnibr.sHtML


<!-- 参考信息 -->