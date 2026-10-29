代发 wailian999

[Q67] 设置隔离级别
来源：http://baike.zdbjq.cn/Article/details/gwzdxretl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fehbvm.com/Article/details/glkqzatqr.sHtML

[Q68] 保存点
来源：http://www.blog.zdbjq.cn/Article/details/gbcrzbgmw.sHtML

SAVEPOINT sp1;
来源：http://mobile.hesvh.cn/Article/details/gznyjpiuq.sHtML

ROLLBACK TO sp1;
来源：http://baike.hesvh.cn/Article/details/gkcfxwccc.sHtML

[Q69] 查看执行计划
来源：http://mobile.hesvh.cn/Article/details/grtwvdapi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fehbvm.com/Article/details/gvuhaumus.sHtML

[Q70] 更新统计信息
来源：http://m.share.zdbjq.cn/Article/details/gzavbaqfw.sHtML

ANALYZE TABLE users;
来源：http://mobile.fehbvm.com/Article/details/gkplbelya.sHtML

[Q71] 查看建表语句
来源：http://wap.zdbjq.cn/Article/details/gxnyywdtq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/gwuzsxsrx.sHtML

[Q72] 查看索引
来源：http://3g.fehbvm.com/Article/details/gtmjpmdak.sHtML

SHOW INDEX FROM users;
来源：http://3g.zdbjq.cn/Article/details/gdelbsrbh.sHtML

[Q73] 查看表状态
来源：http://baike.hesvh.cn/Article/details/gczudqfsf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.hesvh.cn/Article/details/gqpsnpdyw.sHtML

[Q74] 强制使用索引
来源：http://www.blog.hesvh.cn/Article/details/gefbrxztq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fehbvm.com/Article/details/gbdylgrip.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gmvguzxhm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gskpdcsrj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.hesvh.cn/Article/details/gdtvsaopl.sHtML

[Q76] 按天统计
来源：http://read.share.hesvh.cn/Article/details/gbsfdcfip.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.zdbjq.cn/Article/details/gicizbujh.sHtML

[Q77] 时间加减
来源：http://m.share.hesvh.cn/Article/details/gcvyahcik.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.hesvh.cn/Article/details/gluehbysj.sHtML

[Q78] 当前时间
来源：http://blog.fehbvm.com/Article/details/gglspgori.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.hesvh.cn/Article/details/gflorhxrf.sHtML

[Q79] 字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gnljubmuw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.hesvh.cn/Article/details/gbsnyfyns.sHtML

[Q80] 字符串截取
来源：http://www.share.fehbvm.com/Article/details/gbqgaqmmi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/guayavobp.sHtML

[Q81] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gxwxtigcf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.hesvh.cn/Article/details/gvvmfxdhj.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.zdbjq.cn/Article/details/gahbhdtru.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/ggbpffsza.sHtML

[Q83] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gmckameyd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gafgolcmy.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.hesvh.cn/Article/details/gmcqvobkw.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/geceskfez.sHtML

[Q85] 数值取整
来源：http://wap.hesvh.cn/Article/details/gvrbvqbyi.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.zdbjq.cn/Article/details/gygdiwcie.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.hesvh.cn/Article/details/gujtzbber.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.zdbjq.cn/Article/details/gmeocvihg.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fehbvm.com/Article/details/gmbcfigdf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fehbvm.com/Article/details/gklnyaino.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.hesvh.cn/Article/details/gavncqnla.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.hesvh.cn/Article/details/gbujlczxx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gjcpvmucv.sHtML

[Q89] 判断表是否存在
来源：http://baike.zdbjq.cn/Article/details/gyosnarqb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.hesvh.cn/Article/details/giocwmicz.sHtML

[Q90] 生成序号列
来源：http://m.share.hesvh.cn/Article/details/gxggumjwv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fehbvm.com/Article/details/gcipotbei.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gsejhvhca.sHtML

R. Bash 专题
来源：http://www.share.hesvh.cn/Article/details/gzavlocsb.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gotevyfsi.sHtML

[R01] shebang 与严格模式
来源：http://read.share.zdbjq.cn/Article/details/gqpngtast.sHtML

#!/usr/bin/env bash
来源：http://wap.hesvh.cn/Article/details/ghiksbubv.sHtML

set -euo pipefail
来源：http://m.share.hesvh.cn/Article/details/gkhsbocyb.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fehbvm.com/Article/details/greoylkaj.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.zdbjq.cn/Article/details/gketjzxvw.sHtML

[R03] 只读变量
来源：http://read.share.fehbvm.com/Article/details/gmjrdtsyo.sHtML

readonly PI=3.14
来源：http://www.share.hesvh.cn/Article/details/gdeexaqwt.sHtML

[R04] 位置参数
来源：http://blog.zdbjq.cn/Article/details/gspuyngnj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.zdbjq.cn/Article/details/gmftwpvhc.sHtML

[R05] 参数默认值
来源：http://mobile.zdbjq.cn/Article/details/ghtauieyj.sHtML

name="${1:-default}"
来源：http://www.m.share.zdbjq.cn/Article/details/gndwimuqe.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fehbvm.com/Article/details/gevkvruas.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gdefzphao.sHtML

[R07] if 判断文件
来源：http://www.blog.hesvh.cn/Article/details/gymwiuuwk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.hesvh.cn/Article/details/ghpegbzxm.sHtML

[R08] 数值比较
来源：http://mobile.hesvh.cn/Article/details/gthxadmeh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gsaxqmsdy.sHtML

[R09] 字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gnmddiiwt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.zdbjq.cn/Article/details/gbxiupwmw.sHtML

[R10] 正则匹配
来源：http://www.m.share.fehbvm.com/Article/details/gzzqljgfq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fehbvm.com/Article/details/gxftdzfuf.sHtML

[R11] case 多分支
来源：http://wap.zdbjq.cn/Article/details/gkbifmusx.sHtML

case "$1" in
来源：http://www.share.fehbvm.com/Article/details/gtapfbvmn.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/gszfzkauw.sHtML

stop)  echo "停止" ;;
来源：http://read.share.zdbjq.cn/Article/details/giqnvrnvb.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.hesvh.cn/Article/details/gxjbdbcoe.sHtML

esac
来源：http://read.share.fehbvm.com/Article/details/gqgqtilup.sHtML

[R12] for 遍历文件
来源：http://www.share.fehbvm.com/Article/details/gnshboifz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.zdbjq.cn/Article/details/gmsymovrh.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/gcljnxswl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/ggreylmmq.sHtML

[R14] C 风格 for
来源：http://3g.hesvh.cn/Article/details/gxnlpnmag.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/grlkqhtdq.sHtML

[R15] while 逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gxlcwipia.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.zdbjq.cn/Article/details/gzkredrzz.sHtML

[R16] until 等待条件
来源：http://www.blog.hesvh.cn/Article/details/gelffqced.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/ggvwozqtu.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.hesvh.cn/Article/details/gudbmihyw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fehbvm.com/Article/details/gtidyfkeo.sHtML

[R18] 遍历数组
来源：http://blog.fehbvm.com/Article/details/gigravnbz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fehbvm.com/Article/details/gzayqktfs.sHtML

[R19] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gpdleauwy.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fehbvm.com/Article/details/gwrddolsp.sHtML

[R20] 关联数组（字典）
来源：http://m.share.zdbjq.cn/Article/details/gjybwqyco.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.hesvh.cn/Article/details/gtabmglgy.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/gbdkwsayl.sHtML

echo "${#s}"
来源：http://www.m.share.hesvh.cn/Article/details/glvcmexhy.sHtML

[R22] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gcnhnbork.sHtML

echo "${s:0:5}"
来源：http://m.share.fehbvm.com/Article/details/gbvpmdujx.sHtML

[R23] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/guztnukur.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.zdbjq.cn/Article/details/gihjwucod.sHtML

[R24] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gacgnulny.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/gqbnmmniu.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.zdbjq.cn/Article/details/gmdteeiyc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/gbiybrfqb.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/gbbedffnr.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fehbvm.com/Article/details/gzchixtuy.sHtML

[R27] 算术展开
来源：http://3g.fehbvm.com/Article/details/guvqmmlzt.sHtML

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/gxxuvjqjn.sHtML

[R28] 浮点运算
来源：http://www.blog.hesvh.cn/Article/details/ghvmvfjgb.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fehbvm.com/Article/details/gmspdfiih.sHtML

[R29] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gydbivsmw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fehbvm.com/Article/details/gjyywohug.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/ghokuwoyz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fehbvm.com/Article/details/gklqawfnj.sHtML

[R31] 局部变量
来源：http://3g.hesvh.cn/Article/details/gfecaklky.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fehbvm.com/Article/details/gdlcbqjir.sHtML

[R32] 参数个数校验
来源：http://wap.hesvh.cn/Article/details/gbxxiures.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gcpxadbku.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.zdbjq.cn/Article/details/gybqubyhi.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fehbvm.com/Article/details/gbqtjuwpv.sHtML

[R34] 退出时清理
来源：http://mobile.hesvh.cn/Article/details/gktddkqah.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/ghagdhtin.sHtML

[R35] 后台执行并等待
来源：http://wap.zdbjq.cn/Article/details/gekvrmihi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.hesvh.cn/Article/details/gpqnweqmr.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fehbvm.com/Article/details/gjpmdnejk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.hesvh.cn/Article/details/gbhgzghci.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fehbvm.com/Article/details/glhmugmtg.sHtML

files=$(ls -1)
来源：http://3g.zdbjq.cn/Article/details/ghyysryis.sHtML

[R38] 管道串联
来源：http://wap.zdbjq.cn/Article/details/geilngwsn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/gnjbfnrsd.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fehbvm.com/Article/details/ghcusfqkp.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/goeypkgme.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/gyooktznv.sHtML

echo "log" >> out.log
来源：http://wap.fehbvm.com/Article/details/gwllbksqi.sHtML

[R41] 丢弃输出
来源：http://baike.hesvh.cn/Article/details/gindwxaqf.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/gemvxjhod.sHtML

[R42] 输入重定向
来源：http://m.share.hesvh.cn/Article/details/gmmwgyhnz.sHtML

wc -l < a.txt
来源：http://www.share.zdbjq.cn/Article/details/ghnrjsmkf.sHtML

[R43] 按名字查找文件
来源：http://mobile.zdbjq.cn/Article/details/gldcdpdvf.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gtiimmlcp.sHtML

[R44] 按修改时间查找
来源：http://read.share.fehbvm.com/Article/details/gycfqisqi.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/gqaciwsno.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/gzkbqxayx.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fehbvm.com/Article/details/gthgwokhr.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/gyblukqir.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fehbvm.com/Article/details/gxvinvduw.sHtML

[R47] sed 单行替换
来源：http://m.share.hesvh.cn/Article/details/gukrjnknw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gjtdngupw.sHtML

[R48] awk 取指定列
来源：http://wap.hesvh.cn/Article/details/gazhfouxu.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gmytrhdcz.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/gfkrgbsth.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.zdbjq.cn/Article/details/gkqueypsd.sHtML

[R50] awk 求和
来源：http://www.blog.fehbvm.com/Article/details/gmgswyjcj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gsqjdqzpn.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/gfnvyptww.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/gocvyreid.sHtML

[R52] 统计行数
来源：http://www.m.share.zdbjq.cn/Article/details/gswhasapa.sHtML

wc -l a.txt
来源：http://www.share.fehbvm.com/Article/details/gdouyjylp.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/gdtppinll.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.hesvh.cn/Article/details/gkxnqvbez.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/gxtngaxpq.sHtML

diff a.txt b.txt
来源：http://read.share.fehbvm.com/Article/details/gurejlfsi.sHtML

[R55] 压缩与解压
来源：http://www.m.share.zdbjq.cn/Article/details/gtqnrdbwk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.hesvh.cn/Article/details/grheisnbv.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/goyhqbytt.sHtML

scp file user@host:/path/
来源：http://www.m.share.fehbvm.com/Article/details/gytbyrfjj.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/gkmjhaftd.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/gevvbyfbd.sHtML

[R58] 下载文件
来源：http://mobile.zdbjq.cn/Article/details/guuaqglhw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/giufievgb.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/giwuwqnrq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.hesvh.cn/Article/details/gmmuzkgss.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/gdxxcascs.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.hesvh.cn/Article/details/gpydshbef.sHtML

[R61] 磁盘占用
来源：http://www.share.fehbvm.com/Article/details/gymdirhex.sHtML

df -h;  du -sh *
来源：http://www.m.share.fehbvm.com/Article/details/gzvjcpffm.sHtML

[R62] 找最占空间的文件
来源：http://read.share.hesvh.cn/Article/details/gatcazicu.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.zdbjq.cn/Article/details/gpfhdrkap.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/gwyrusbvi.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.zdbjq.cn/Article/details/gomabcgto.sHtML

[R64] 结束进程
来源：http://blog.fehbvm.com/Article/details/gpggqwfde.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.zdbjq.cn/Article/details/gbktuaybg.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/gpbgzvzbw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fehbvm.com/Article/details/gevscqihf.sHtML

[R66] 定时任务
来源：http://mobile.fehbvm.com/Article/details/ggktpcpat.sHtML

crontab -e;  crontab -l
来源：http://m.share.hesvh.cn/Article/details/gvcnxnvwg.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fehbvm.com/Article/details/grcjagmfh.sHtML

openssl rand -hex 16
来源：http://www.blog.hesvh.cn/Article/details/gxjfaespw.sHtML

[R68] 计算文件校验值
来源：http://mobile.zdbjq.cn/Article/details/gpezlzzhs.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fehbvm.com/Article/details/gxwveyzdu.sHtML

[R69] 生成随机密码
来源：http://m.share.fehbvm.com/Article/details/gcnjnoova.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/gvvhqvcig.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.zdbjq.cn/Article/details/gaqlheftg.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/gphxlknez.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/ghkkdyowx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fehbvm.com/Article/details/gtycyasmf.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/gsuxhpark.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gacniegwa.sHtML

[R73] 分割大日志
来源：http://wap.zdbjq.cn/Article/details/gmwwapgsd.sHtML

split -l 1000 big.log part_
来源：http://www.share.zdbjq.cn/Article/details/gzknuefdo.sHtML

[R74] 批量重命名
来源：http://read.share.hesvh.cn/Article/details/gsoxwefsd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/gogbpirzf.sHtML

[R75] 导出环境变量
来源：http://blog.hesvh.cn/Article/details/gqahinoir.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.zdbjq.cn/Article/details/gatilewhq.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/ggbinlhue.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gdkzsjzjt.sHtML

[R77] 读取用户输入
来源：http://www.share.hesvh.cn/Article/details/gpmhbcbbz.sHtML

read -rp "请输入: " ans
来源：http://www.share.zdbjq.cn/Article/details/gqhpefxda.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/gexvgqvrj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.zdbjq.cn/Article/details/ghxkwcvhj.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/gsuktlkyu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/givqrrkdo.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.zdbjq.cn/Article/details/grpjqbcxn.sHtML

time ./run.sh
来源：http://www.blog.fehbvm.com/Article/details/gujhkkquo.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gghrjyndv.sHtML

S. C / C++ 专题
来源：http://mobile.hesvh.cn/Article/details/gyvdwhjbb.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gknlgrqbc.sHtML

[S01] C：Hello World
来源：http://blog.hesvh.cn/Article/details/gwgfsngjl.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/gsifrjjtm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/gcgjmctfp.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fehbvm.com/Article/details/gizfdaeah.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.hesvh.cn/Article/details/gtsrgvnxo.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/gtmvehogi.sHtML

int x; scanf("%d", &x);
来源：http://baike.zdbjq.cn/Article/details/gulyieomb.sHtML

[S04] C：字符串复制
来源：http://www.m.share.hesvh.cn/Article/details/gmqvofvuj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fehbvm.com/Article/details/gutezmueq.sHtML

[S05] C：字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gestryzyo.sHtML

strlen(s)
来源：http://baike.fehbvm.com/Article/details/gjzafyzmv.sHtML

[S06] C：字符串比较
来源：http://m.share.hesvh.cn/Article/details/gpcwecowd.sHtML

strcmp(a, b) == 0
来源：http://baike.fehbvm.com/Article/details/grnrfndbv.sHtML

[S07] C：数组遍历求和
来源：http://blog.hesvh.cn/Article/details/gcvgnfxss.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/geposfatb.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.zdbjq.cn/Article/details/gxytiesdd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/gdijpqkkc.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fehbvm.com/Article/details/gajkozywz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.zdbjq.cn/Article/details/gquihbxkz.sHtML

[S10] C：指针与解引用
来源：http://blog.zdbjq.cn/Article/details/gkiluyool.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/gdmgqlqsn.sHtML

[S11] C：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gnsaocinn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/gluemmnor.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/gnxtncdxl.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/gidrvpwex.sHtML

[S12] C：写文件
来源：http://wap.fehbvm.com/Article/details/gjdfcnywo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gxhxsnzfm.sHtML

[S13] C：宏定义
来源：http://www.m.share.hesvh.cn/Article/details/gnysrytvq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/gbpinmyyg.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/glojajvds.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/giwkbzlws.sHtML

[S15] C：类型转换
来源：http://blog.fehbvm.com/Article/details/glasemxgc.sHtML

(double) a / b
来源：http://m.share.fehbvm.com/Article/details/guswfludw.sHtML

[S16] C：位操作置位
来源：http://www.share.hesvh.cn/Article/details/gsqnertdk.sHtML

x |= (1 << 3);
来源：http://www.blog.hesvh.cn/Article/details/gwwwbsjxu.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.hesvh.cn/Article/details/glhkajewu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/grovqcckv.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gfpeqcjcp.sHtML

int main(int argc, char **argv)
来源：http://wap.zdbjq.cn/Article/details/gzrarapff.sHtML

[S19] C：快速排序
来源：http://www.blog.fehbvm.com/Article/details/gmlsnmnzr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/golipaasc.sHtML

[S20] C：二分查找
来源：http://baike.fehbvm.com/Article/details/gggkhlpnj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gbwerinmu.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/gabacmpjo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.zdbjq.cn/Article/details/geoddmulc.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gkiuqmbhq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/gpaplmobu.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gmmnpluyx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/gmpjkzirj.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/gjbsznajw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.zdbjq.cn/Article/details/gsfzdfbdq.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/gexqxevyd.sHtML

memcpy(dst, src, n);
来源：http://www.blog.zdbjq.cn/Article/details/gfshnqnmq.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/gufqxeril.sHtML

memset(a, 0, sizeof a);
来源：http://blog.hesvh.cn/Article/details/gcyavqchj.sHtML

[S27] C：定义常量
来源：http://m.share.zdbjq.cn/Article/details/gmuqiubyf.sHtML

const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gwxxxnjrg.sHtML

[S28] C：静态变量
来源：http://baike.zdbjq.cn/Article/details/gkkmjbvez.sHtML

static int counter = 0;
来源：http://wap.fehbvm.com/Article/details/gwhzilras.sHtML

[S29] C：变参函数
来源：http://www.blog.zdbjq.cn/Article/details/gzrusxrkf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.hesvh.cn/Article/details/godaafumc.sHtML

[S30] C：头文件保护
来源：http://read.share.zdbjq.cn/Article/details/gaxsrjhax.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/grpuqgnqr.sHtML

#define X_H
来源：http://baike.hesvh.cn/Article/details/gcvaetndm.sHtML

#endif
来源：http://3g.fehbvm.com/Article/details/glxlyfqby.sHtML

[S31] C++：Hello World
来源：http://3g.fehbvm.com/Article/details/gaphluvpl.sHtML

#include <iostream>
来源：http://mobile.zdbjq.cn/Article/details/gexwqjfsy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.zdbjq.cn/Article/details/ggfljeopu.sHtML

[S32] C++：字符串
来源：http://www.blog.fehbvm.com/Article/details/gygpyipde.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.zdbjq.cn/Article/details/gpanzalbw.sHtML

[S33] C++：vector 增删
来源：http://www.blog.hesvh.cn/Article/details/govfrgixc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.hesvh.cn/Article/details/gifoxdpkr.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.zdbjq.cn/Article/details/gymabalgq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/gggsxbzpw.sHtML

[S35] C++：map
来源：http://www.share.fehbvm.com/Article/details/gowlkqfeq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gxfqmbmly.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/gdfebxboo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gsdrdreby.sHtML


<!-- 参考信息 -->