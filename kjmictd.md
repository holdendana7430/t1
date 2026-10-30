代发 wailian999

[Q65] 回滚事务
来源：http://blog.fehbvm.com/Article/details/gzfoeazvc.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/gbjbkzzel.sHtML

[Q66] 行锁查询
来源：http://wap.zdbjq.cn/Article/details/gbaxgtryf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.hesvh.cn/Article/details/gwzrzrhsb.sHtML

[Q67] 设置隔离级别
来源：http://baike.hesvh.cn/Article/details/gjgwjqlsl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.hesvh.cn/Article/details/gqjnqfkzw.sHtML

[Q68] 保存点
来源：http://mobile.zdbjq.cn/Article/details/gcvzifldx.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/giepnavyt.sHtML

ROLLBACK TO sp1;
来源：http://read.share.zdbjq.cn/Article/details/gbvxsgppt.sHtML

[Q69] 查看执行计划
来源：http://m.share.hesvh.cn/Article/details/gsknmmcst.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.zdbjq.cn/Article/details/gchjmlvdw.sHtML

[Q70] 更新统计信息
来源：http://read.share.zdbjq.cn/Article/details/gdafxawmz.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fehbvm.com/Article/details/gmdcfhevi.sHtML

[Q71] 查看建表语句
来源：http://www.share.fehbvm.com/Article/details/gxisgfwwd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.zdbjq.cn/Article/details/gvgkcycqj.sHtML

[Q72] 查看索引
来源：http://blog.zdbjq.cn/Article/details/gxxkuwusv.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/gjfzjmpco.sHtML

[Q73] 查看表状态
来源：http://www.share.zdbjq.cn/Article/details/gmwvffbwh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fehbvm.com/Article/details/grtmvdovt.sHtML

[Q74] 强制使用索引
来源：http://mobile.fehbvm.com/Article/details/gfgzkrgqr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.hesvh.cn/Article/details/gklyuvuhu.sHtML

[Q75] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gitbncxbs.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gbtacravd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.zdbjq.cn/Article/details/gdprmzjpy.sHtML

[Q76] 按天统计
来源：http://read.share.hesvh.cn/Article/details/goabkqxch.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fehbvm.com/Article/details/gytbuhetg.sHtML

[Q77] 时间加减
来源：http://www.m.share.zdbjq.cn/Article/details/gjyrkcxlx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.zdbjq.cn/Article/details/gsvnmxxko.sHtML

[Q78] 当前时间
来源：http://m.share.zdbjq.cn/Article/details/gunqdpblx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.zdbjq.cn/Article/details/grxanogkc.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/grjqxmsws.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.hesvh.cn/Article/details/ghtnfmidn.sHtML

[Q80] 字符串截取
来源：http://read.share.hesvh.cn/Article/details/gmqsfymrj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fehbvm.com/Article/details/glkitqvbi.sHtML

[Q81] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gmatvjnmz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gxxnolyxu.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fehbvm.com/Article/details/gzlzlcpoe.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gixofonvh.sHtML

[Q83] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gawfzguhs.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gannnunuy.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.hesvh.cn/Article/details/gbepbxugn.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gfavkngex.sHtML

[Q85] 数值取整
来源：http://www.m.share.zdbjq.cn/Article/details/ggpdzjbxv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.zdbjq.cn/Article/details/gaaernjut.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fehbvm.com/Article/details/gzcqawnei.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fehbvm.com/Article/details/grhnbqbai.sHtML

[Q87] JSON 字段做条件
来源：http://baike.zdbjq.cn/Article/details/gwozxlrsi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.zdbjq.cn/Article/details/gzqfgxinf.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.zdbjq.cn/Article/details/guymhmnir.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.zdbjq.cn/Article/details/ggbxprbac.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gfinkwejw.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/gguknolaw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.zdbjq.cn/Article/details/gwamtbymt.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/gqkjdvxdm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fehbvm.com/Article/details/gmkifrjvw.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gegrnarnn.sHtML

R. Bash 专题
来源：http://read.share.zdbjq.cn/Article/details/gvdcxljkf.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gzffhfzuo.sHtML

[R01] shebang 与严格模式
来源：http://3g.zdbjq.cn/Article/details/gqvldgzmo.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.hesvh.cn/Article/details/ghosobhgk.sHtML

set -euo pipefail
来源：http://blog.zdbjq.cn/Article/details/goxavcrtn.sHtML

[R02] 变量赋值与使用
来源：http://3g.fehbvm.com/Article/details/gjndldojp.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fehbvm.com/Article/details/guxnqauxi.sHtML

[R03] 只读变量
来源：http://blog.fehbvm.com/Article/details/gedgmyubi.sHtML

readonly PI=3.14
来源：http://www.blog.fehbvm.com/Article/details/gfqxbwvoz.sHtML

[R04] 位置参数
来源：http://www.blog.zdbjq.cn/Article/details/gerwnjzls.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.zdbjq.cn/Article/details/ghaiwdwtd.sHtML

[R05] 参数默认值
来源：http://www.share.hesvh.cn/Article/details/gkkrsmhyn.sHtML

name="${1:-default}"
来源：http://m.share.zdbjq.cn/Article/details/gfswjbpja.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.hesvh.cn/Article/details/gwqoiiuek.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gynyupflo.sHtML

[R07] if 判断文件
来源：http://3g.hesvh.cn/Article/details/gekwltdfs.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.zdbjq.cn/Article/details/gvjuwrprp.sHtML

[R08] 数值比较
来源：http://m.share.hesvh.cn/Article/details/gwdjuslye.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.hesvh.cn/Article/details/gtpjpwyic.sHtML

[R09] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gionwdviw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.hesvh.cn/Article/details/grdyczdqp.sHtML

[R10] 正则匹配
来源：http://3g.hesvh.cn/Article/details/grreadoze.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.zdbjq.cn/Article/details/gzitmpkrn.sHtML

[R11] case 多分支
来源：http://www.share.hesvh.cn/Article/details/gbvwccdjv.sHtML

case "$1" in
来源：http://www.blog.zdbjq.cn/Article/details/gaammeosp.sHtML

start) echo "启动" ;;
来源：http://wap.fehbvm.com/Article/details/geneyuqkz.sHtML

stop)  echo "停止" ;;
来源：http://wap.fehbvm.com/Article/details/gihffupig.sHtML

*)     echo "未知命令" ;;
来源：http://blog.zdbjq.cn/Article/details/gawyycrpa.sHtML

esac
来源：http://baike.zdbjq.cn/Article/details/gnjsijvki.sHtML

[R12] for 遍历文件
来源：http://blog.fehbvm.com/Article/details/geatxvnxg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.hesvh.cn/Article/details/gpdgauyxb.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gsevkxkyd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gwdchqxuv.sHtML

[R14] C 风格 for
来源：http://mobile.zdbjq.cn/Article/details/gyvnbaynj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gqutjsdxa.sHtML

[R15] while 逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gfktxwils.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gnhvqjxxh.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/gdyatdxlz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/guxndwxux.sHtML

[R17] 数组定义与取值
来源：http://m.share.hesvh.cn/Article/details/gttrlikuv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.hesvh.cn/Article/details/gogmjrouo.sHtML

[R18] 遍历数组
来源：http://read.share.hesvh.cn/Article/details/gwjmdwqgy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.hesvh.cn/Article/details/geiuovenq.sHtML

[R19] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gsvkscqbh.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/gkinmzryc.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.hesvh.cn/Article/details/gnxzltzan.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.zdbjq.cn/Article/details/gdpbftppp.sHtML

[R21] 字符串长度
来源：http://blog.zdbjq.cn/Article/details/gdwuszghx.sHtML

echo "${#s}"
来源：http://www.share.hesvh.cn/Article/details/ghozlucji.sHtML

[R22] 截取子串
来源：http://m.share.fehbvm.com/Article/details/giwxwushd.sHtML

echo "${s:0:5}"
来源：http://read.share.fehbvm.com/Article/details/gvqvtjspv.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gapzggskw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/gcgmbmksr.sHtML

[R24] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gxqoeoeus.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/gtbbpvtca.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.hesvh.cn/Article/details/gxoeyjuxv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.zdbjq.cn/Article/details/gysolttok.sHtML

[R26] 命令替换
来源：http://m.share.fehbvm.com/Article/details/gooesspcu.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/gpenwfgfc.sHtML

[R27] 算术展开
来源：http://m.share.hesvh.cn/Article/details/gzakompic.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/gdsijxezm.sHtML

[R28] 浮点运算
来源：http://www.blog.hesvh.cn/Article/details/gbomlutmr.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.hesvh.cn/Article/details/gyixmhilr.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/gwuomwija.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fehbvm.com/Article/details/gwybsdfuz.sHtML

[R30] 函数返回状态码
来源：http://read.share.zdbjq.cn/Article/details/giqixkomu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.zdbjq.cn/Article/details/gbbnusyzl.sHtML

[R31] 局部变量
来源：http://m.share.hesvh.cn/Article/details/ghrfsfhzp.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.zdbjq.cn/Article/details/gvpfpgkhg.sHtML

[R32] 参数个数校验
来源：http://read.share.hesvh.cn/Article/details/goponwmno.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gczoowwnk.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fehbvm.com/Article/details/gmexyywvs.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fehbvm.com/Article/details/gjmncbper.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/grazqlxzt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gjlrdrunh.sHtML

[R35] 后台执行并等待
来源：http://3g.fehbvm.com/Article/details/gplhcmsvk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/gehcildho.sHtML

[R36] 并发执行多个任务
来源：http://blog.zdbjq.cn/Article/details/gdvdddjgh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fehbvm.com/Article/details/gcieofhbn.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fehbvm.com/Article/details/gwfqlrfpf.sHtML

files=$(ls -1)
来源：http://read.share.fehbvm.com/Article/details/grgvvzheu.sHtML

[R38] 管道串联
来源：http://blog.zdbjq.cn/Article/details/ggnjzhlva.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/gjkhumgde.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.hesvh.cn/Article/details/gtazdwzyg.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gruhfvspw.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/grxssllaz.sHtML

echo "log" >> out.log
来源：http://www.share.fehbvm.com/Article/details/gzlzmhhrv.sHtML

[R41] 丢弃输出
来源：http://blog.zdbjq.cn/Article/details/gpersxjjg.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gcdqhsmim.sHtML

[R42] 输入重定向
来源：http://wap.zdbjq.cn/Article/details/gkiljlokx.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/giuzgsplg.sHtML

[R43] 按名字查找文件
来源：http://baike.hesvh.cn/Article/details/gzchhgzet.sHtML

find . -name "*.log" -type f
来源：http://wap.fehbvm.com/Article/details/gqgtcngyj.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/gcmukgpjs.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fehbvm.com/Article/details/gveaouaaj.sHtML

[R45] 批量删除
来源：http://www.share.fehbvm.com/Article/details/gbnrbswzm.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.zdbjq.cn/Article/details/gvuynnfxv.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fehbvm.com/Article/details/gtlvamvoj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.zdbjq.cn/Article/details/gswlweqen.sHtML

[R47] sed 单行替换
来源：http://baike.hesvh.cn/Article/details/gjaitxzeg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.zdbjq.cn/Article/details/getwrtmhf.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/gezekjkhs.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gchoqytze.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/guhfacwoc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.zdbjq.cn/Article/details/guuxihshz.sHtML

[R50] awk 求和
来源：http://baike.hesvh.cn/Article/details/grrehprtm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gmbpzybsy.sHtML

[R51] 排序去重取前几
来源：http://m.share.zdbjq.cn/Article/details/gqllobmwg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.zdbjq.cn/Article/details/gvvoymtyv.sHtML

[R52] 统计行数
来源：http://baike.zdbjq.cn/Article/details/gruvyjvqg.sHtML

wc -l a.txt
来源：http://blog.hesvh.cn/Article/details/gwfpllgwq.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/gecmiunrx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.hesvh.cn/Article/details/gzhcpzqlt.sHtML

[R54] 比较两个文件
来源：http://3g.fehbvm.com/Article/details/gwurgkbgw.sHtML

diff a.txt b.txt
来源：http://www.m.share.fehbvm.com/Article/details/gyforwxfq.sHtML

[R55] 压缩与解压
来源：http://3g.fehbvm.com/Article/details/ggkzbbnqf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/geiascpsv.sHtML

[R56] 远程拷贝
来源：http://www.share.hesvh.cn/Article/details/ghhuffnaa.sHtML

scp file user@host:/path/
来源：http://3g.fehbvm.com/Article/details/grnohytaf.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/gbdknvzpe.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/gbwbrernb.sHtML

[R58] 下载文件
来源：http://wap.fehbvm.com/Article/details/gessvsntl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/gdkhqlkgn.sHtML

[R59] 发 POST JSON
来源：http://wap.hesvh.cn/Article/details/ggizljgts.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.hesvh.cn/Article/details/gyysocglj.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gjkekdeko.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fehbvm.com/Article/details/gwtqtnslq.sHtML

[R61] 磁盘占用
来源：http://www.share.zdbjq.cn/Article/details/gsvkibbcn.sHtML

df -h;  du -sh *
来源：http://baike.fehbvm.com/Article/details/gbnwdloxp.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/garstfzho.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.hesvh.cn/Article/details/gngmuhsqu.sHtML

[R63] 内存与进程
来源：http://blog.zdbjq.cn/Article/details/ghzzzkocv.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.hesvh.cn/Article/details/gfdzeywud.sHtML

[R64] 结束进程
来源：http://mobile.fehbvm.com/Article/details/gutiqgthb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/gjigxmqik.sHtML

[R65] 查看端口占用
来源：http://wap.fehbvm.com/Article/details/geqhnwbhz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.zdbjq.cn/Article/details/gkebzrkoi.sHtML

[R66] 定时任务
来源：http://blog.fehbvm.com/Article/details/gyyfigfod.sHtML

crontab -e;  crontab -l
来源：http://m.share.hesvh.cn/Article/details/gthytbqrp.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/guyywevei.sHtML

openssl rand -hex 16
来源：http://mobile.zdbjq.cn/Article/details/ghrzlxpdq.sHtML

[R68] 计算文件校验值
来源：http://m.share.zdbjq.cn/Article/details/gngslujwg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.zdbjq.cn/Article/details/gpxcoflsd.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/gdqqvptjs.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.zdbjq.cn/Article/details/glnnnecpk.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/gzzaysoed.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fehbvm.com/Article/details/gogkqkekb.sHtML

[R71] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gtugqqhrs.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.zdbjq.cn/Article/details/gqskfwfvf.sHtML

[R72] 等待端口就绪
来源：http://blog.hesvh.cn/Article/details/gbgnqtgsh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gmturadai.sHtML

[R73] 分割大日志
来源：http://www.share.hesvh.cn/Article/details/gtucnczkk.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.hesvh.cn/Article/details/gfollzhxn.sHtML

[R74] 批量重命名
来源：http://www.m.share.fehbvm.com/Article/details/gfpmfjwhd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.zdbjq.cn/Article/details/giezizppg.sHtML

[R75] 导出环境变量
来源：http://blog.fehbvm.com/Article/details/gdysjygpu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.hesvh.cn/Article/details/grvxyepcy.sHtML

[R76] 使用临时文件
来源：http://mobile.zdbjq.cn/Article/details/gsuifdzxw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gsmlvzhls.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/gsvzhucoq.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/geibydbsr.sHtML

[R78] 交互式菜单
来源：http://wap.fehbvm.com/Article/details/gpkhbskdt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/gqhoridfv.sHtML

[R79] 解析命令行选项
来源：http://www.blog.hesvh.cn/Article/details/gvsaxuxqo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.hesvh.cn/Article/details/gnimyihge.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/gtfxhmwmi.sHtML

time ./run.sh
来源：http://read.share.zdbjq.cn/Article/details/gipbbijtf.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfmenckzl.sHtML

S. C / C++ 专题
来源：http://baike.hesvh.cn/Article/details/gtljsrrcx.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjczeelkv.sHtML

[S01] C：Hello World
来源：http://www.share.fehbvm.com/Article/details/gdrfhbxpo.sHtML

#include <stdio.h>
来源：http://www.blog.hesvh.cn/Article/details/gwjxgifrh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.hesvh.cn/Article/details/gwtqclolr.sHtML

[S02] C：变量与格式化输出
来源：http://3g.zdbjq.cn/Article/details/gzlgiclfe.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/ggxwafchy.sHtML

[S03] C：读入整数
来源：http://blog.zdbjq.cn/Article/details/gudjzxebw.sHtML

int x; scanf("%d", &x);
来源：http://wap.hesvh.cn/Article/details/gzcwyjlwd.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/geankwnvs.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gklxzqstx.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gbpbpedca.sHtML

strlen(s)
来源：http://mobile.hesvh.cn/Article/details/gghbqivru.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/gdsyyfzxj.sHtML

strcmp(a, b) == 0
来源：http://www.share.fehbvm.com/Article/details/gppaibrwi.sHtML

[S07] C：数组遍历求和
来源：http://www.share.zdbjq.cn/Article/details/gwarjwpag.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/gkewzjrpk.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.hesvh.cn/Article/details/gqzezhpiy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fehbvm.com/Article/details/gvgzyxcnw.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.zdbjq.cn/Article/details/gvwyeaiyk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/gkpsdtydo.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/garardcmx.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fehbvm.com/Article/details/gdpqhwwck.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gablkvxte.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fehbvm.com/Article/details/gvzutphwt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.hesvh.cn/Article/details/gmzjjgdjt.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gywdfwydb.sHtML

[S12] C：写文件
来源：http://blog.fehbvm.com/Article/details/gvftfbfxl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gxnnyczjm.sHtML

[S13] C：宏定义
来源：http://www.blog.fehbvm.com/Article/details/gendpdyir.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.zdbjq.cn/Article/details/gepzflvpw.sHtML

[S14] C：枚举
来源：http://mobile.zdbjq.cn/Article/details/gpjdoxxwg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.hesvh.cn/Article/details/gojqotlcs.sHtML

[S15] C：类型转换
来源：http://wap.fehbvm.com/Article/details/gyrgvvfuv.sHtML

(double) a / b
来源：http://www.m.share.zdbjq.cn/Article/details/gzjbxnnyn.sHtML

[S16] C：位操作置位
来源：http://blog.hesvh.cn/Article/details/gngvqnsoa.sHtML

x |= (1 << 3);
来源：http://baike.zdbjq.cn/Article/details/gwgncawul.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gsqfwvluf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.zdbjq.cn/Article/details/giqdjjpin.sHtML

[S18] C：命令行参数
来源：http://blog.zdbjq.cn/Article/details/gzrdnibpj.sHtML

int main(int argc, char **argv)
来源：http://baike.fehbvm.com/Article/details/gdovybtgp.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/gtwaflhqp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gcffmvzmm.sHtML

[S20] C：二分查找
来源：http://www.blog.zdbjq.cn/Article/details/gbgcfitce.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gvkgzkavc.sHtML

[S21] C：字符类别判断
来源：http://www.share.hesvh.cn/Article/details/gzvzpkijw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.hesvh.cn/Article/details/gazfjrtzw.sHtML

[S22] C：字符串转数字
来源：http://baike.fehbvm.com/Article/details/gjqkbxvku.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fehbvm.com/Article/details/gfhcepxjg.sHtML

[S23] C：随机数
来源：http://wap.fehbvm.com/Article/details/gjnwmahtk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/gypahqlob.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/gwpyelztt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.hesvh.cn/Article/details/gyaohgnjk.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/gmhnuofij.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.hesvh.cn/Article/details/gcxrnigpj.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/gczwvfowj.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/gqtxujxnu.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/ghwaqfgxo.sHtML

const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gyeopnhfk.sHtML

[S28] C：静态变量
来源：http://mobile.zdbjq.cn/Article/details/gemjytncz.sHtML

static int counter = 0;
来源：http://3g.hesvh.cn/Article/details/grugjzbxu.sHtML

[S29] C：变参函数
来源：http://3g.hesvh.cn/Article/details/gvuvrxqcn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fehbvm.com/Article/details/gttqmadzr.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/gyvkarydl.sHtML

#ifndef X_H
来源：http://blog.fehbvm.com/Article/details/glyanbdch.sHtML

#define X_H
来源：http://www.m.share.hesvh.cn/Article/details/gflsftrir.sHtML

#endif
来源：http://www.m.share.hesvh.cn/Article/details/gsowcetig.sHtML

[S31] C++：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gwjxocubs.sHtML

#include <iostream>
来源：http://mobile.hesvh.cn/Article/details/gmbzswymg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fehbvm.com/Article/details/gycebuasz.sHtML

[S32] C++：字符串
来源：http://blog.zdbjq.cn/Article/details/glfmmjrha.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.zdbjq.cn/Article/details/gexpacnql.sHtML

[S33] C++：vector 增删
来源：http://mobile.zdbjq.cn/Article/details/gjcbbuzys.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.zdbjq.cn/Article/details/ghkaxbrob.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fehbvm.com/Article/details/gwjutxppi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/gewrdnjlo.sHtML


<!-- 参考信息 -->