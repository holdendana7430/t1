代发 wailian999

[Q67] 设置隔离级别
来源：http://www.blog.hesvh.cn/Article/details/gtfkuacyy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fehbvm.com/Article/details/gqgbypqhb.sHtML

[Q68] 保存点
来源：http://baike.fehbvm.com/Article/details/gyyatofca.sHtML

SAVEPOINT sp1;
来源：http://blog.fehbvm.com/Article/details/gxjkvssxl.sHtML

ROLLBACK TO sp1;
来源：http://m.share.hesvh.cn/Article/details/gfdsqwepb.sHtML

[Q69] 查看执行计划
来源：http://m.share.fehbvm.com/Article/details/gelqcevke.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/gcwklnspa.sHtML

[Q70] 更新统计信息
来源：http://read.share.hesvh.cn/Article/details/gpxlurtcw.sHtML

ANALYZE TABLE users;
来源：http://read.share.hesvh.cn/Article/details/gkomxocaq.sHtML

[Q71] 查看建表语句
来源：http://m.share.hesvh.cn/Article/details/gqfdijhmf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.hesvh.cn/Article/details/gnxaebpxs.sHtML

[Q72] 查看索引
来源：http://www.m.share.hesvh.cn/Article/details/ghwvnyxuo.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gwapnvwpe.sHtML

[Q73] 查看表状态
来源：http://baike.hesvh.cn/Article/details/guzrineuu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gjlkepwjm.sHtML

[Q74] 强制使用索引
来源：http://www.share.hesvh.cn/Article/details/gfugmkcvt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.zdbjq.cn/Article/details/gigeukqhi.sHtML

[Q75] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gywvdcrhf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gerblsjud.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.zdbjq.cn/Article/details/gshbtuflf.sHtML

[Q76] 按天统计
来源：http://blog.zdbjq.cn/Article/details/gxpidjdny.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.hesvh.cn/Article/details/gmgerwlki.sHtML

[Q77] 时间加减
来源：http://baike.hesvh.cn/Article/details/gjyuzmlot.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.hesvh.cn/Article/details/gmgmydlji.sHtML

[Q78] 当前时间
来源：http://www.blog.zdbjq.cn/Article/details/ggbokznrh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.hesvh.cn/Article/details/gmswpovdl.sHtML

[Q79] 字符串拼接
来源：http://wap.zdbjq.cn/Article/details/ghuvvsszv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.zdbjq.cn/Article/details/gfrakmeau.sHtML

[Q80] 字符串截取
来源：http://blog.zdbjq.cn/Article/details/gaorfhtnn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fehbvm.com/Article/details/gzwmwobdj.sHtML

[Q81] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gwqzbdpga.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gashopajn.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.hesvh.cn/Article/details/gnyeccbpc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gszmhyjwa.sHtML

[Q83] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gpjmtantm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gvowzwjgh.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gjysherhs.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gmtxbvekf.sHtML

[Q85] 数值取整
来源：http://www.blog.zdbjq.cn/Article/details/gwcvtqonl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/gnaryjvqg.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.hesvh.cn/Article/details/gkbtazruy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fehbvm.com/Article/details/gowlxiuee.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.zdbjq.cn/Article/details/gjctchpnd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.hesvh.cn/Article/details/genpnasor.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fehbvm.com/Article/details/gfwxysmcs.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.zdbjq.cn/Article/details/ggpadspex.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gdkzlseac.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gmzickjrj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gqswiucvc.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/gvqogkzvl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.hesvh.cn/Article/details/gknhntvgo.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnwmludbk.sHtML

R. Bash 专题
来源：http://read.share.fehbvm.com/Article/details/gmpvpleoj.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtsquvzdb.sHtML

[R01] shebang 与严格模式
来源：http://m.share.hesvh.cn/Article/details/gdxyfzncy.sHtML

#!/usr/bin/env bash
来源：http://blog.zdbjq.cn/Article/details/gcwxxywqp.sHtML

set -euo pipefail
来源：http://mobile.hesvh.cn/Article/details/gxwnlmkwp.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.hesvh.cn/Article/details/gksmmmsli.sHtML

name="Tom"; echo "$name"
来源：http://www.share.zdbjq.cn/Article/details/gbfhyxaac.sHtML

[R03] 只读变量
来源：http://3g.zdbjq.cn/Article/details/gjwfxrfxu.sHtML

readonly PI=3.14
来源：http://blog.zdbjq.cn/Article/details/grvvspevv.sHtML

[R04] 位置参数
来源：http://3g.zdbjq.cn/Article/details/gftvtildz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fehbvm.com/Article/details/gehrlojoz.sHtML

[R05] 参数默认值
来源：http://mobile.hesvh.cn/Article/details/gpeguvjio.sHtML

name="${1:-default}"
来源：http://m.share.zdbjq.cn/Article/details/gwmijoikb.sHtML

[R06] 判断命令是否存在
来源：http://www.share.zdbjq.cn/Article/details/gfdueqlql.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/grqyeapla.sHtML

[R07] if 判断文件
来源：http://wap.hesvh.cn/Article/details/gtplbpyit.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.zdbjq.cn/Article/details/guoopoujv.sHtML

[R08] 数值比较
来源：http://wap.hesvh.cn/Article/details/gbteskxtl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.zdbjq.cn/Article/details/geuvcjeqy.sHtML

[R09] 字符串比较
来源：http://baike.fehbvm.com/Article/details/gbcslzhfc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.hesvh.cn/Article/details/ghzkibrxc.sHtML

[R10] 正则匹配
来源：http://baike.fehbvm.com/Article/details/gqnxlrtlp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gliazaujj.sHtML

[R11] case 多分支
来源：http://www.m.share.zdbjq.cn/Article/details/gzegrogxm.sHtML

case "$1" in
来源：http://baike.zdbjq.cn/Article/details/geqsxxhdd.sHtML

start) echo "启动" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gekounual.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gdzwyenek.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.zdbjq.cn/Article/details/ghpecwyld.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/gwhjbfrxk.sHtML

[R12] for 遍历文件
来源：http://wap.hesvh.cn/Article/details/gqomkyzzh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/gltjrtxzf.sHtML

[R13] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/gekkaqqfb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gwjwilxoh.sHtML

[R14] C 风格 for
来源：http://baike.hesvh.cn/Article/details/gmmafisud.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/glzovjzbz.sHtML

[R15] while 逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gimnisbrd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fehbvm.com/Article/details/gwmnifunr.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/gaiusdcqc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gdzwepeql.sHtML

[R17] 数组定义与取值
来源：http://3g.hesvh.cn/Article/details/guynjttxb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.hesvh.cn/Article/details/gvtdwzxnm.sHtML

[R18] 遍历数组
来源：http://m.share.hesvh.cn/Article/details/gcvldhjxx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/gbxrhiwvd.sHtML

[R19] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gombiqajg.sHtML

echo "${#arr[@]}"
来源：http://m.share.fehbvm.com/Article/details/geylfypdm.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fehbvm.com/Article/details/gdplzxopo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fehbvm.com/Article/details/gvqxqnmyg.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/ghxsswwta.sHtML

echo "${#s}"
来源：http://3g.zdbjq.cn/Article/details/gdcpbfjdh.sHtML

[R22] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gmooxspob.sHtML

echo "${s:0:5}"
来源：http://read.share.fehbvm.com/Article/details/ggdopsxxi.sHtML

[R23] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gwsjexaib.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.hesvh.cn/Article/details/gbfhsming.sHtML

[R24] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gbdrclwrb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.zdbjq.cn/Article/details/gkdgozoug.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.zdbjq.cn/Article/details/gbezcjzwp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.zdbjq.cn/Article/details/ggyonpgsg.sHtML

[R26] 命令替换
来源：http://baike.hesvh.cn/Article/details/ghfspxtcm.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fehbvm.com/Article/details/giafwtvkr.sHtML

[R27] 算术展开
来源：http://baike.zdbjq.cn/Article/details/gpvrxwoie.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/gjejrwuhq.sHtML

[R28] 浮点运算
来源：http://www.blog.hesvh.cn/Article/details/gncalehqj.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.hesvh.cn/Article/details/glxnmnsqa.sHtML

[R29] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gccnpuiog.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/gnpjiarzl.sHtML

[R30] 函数返回状态码
来源：http://m.share.fehbvm.com/Article/details/gslrclxkw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.hesvh.cn/Article/details/gsifbxlnr.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/gjtonnqgt.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.hesvh.cn/Article/details/gohwtrirg.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/ghwdyvmgb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gfskgecjd.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/glvxugsse.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/gvjkrflwq.sHtML

[R34] 退出时清理
来源：http://www.m.share.fehbvm.com/Article/details/gzfcwlyld.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gfeqcqpgd.sHtML

[R35] 后台执行并等待
来源：http://wap.fehbvm.com/Article/details/gxfhwifsa.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.zdbjq.cn/Article/details/gnesxkmif.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fehbvm.com/Article/details/gvhbhwizc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/giynkqncb.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/gwdndutpm.sHtML

files=$(ls -1)
来源：http://blog.fehbvm.com/Article/details/gtkbfzwev.sHtML

[R38] 管道串联
来源：http://www.m.share.zdbjq.cn/Article/details/gfcrrjtfi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.hesvh.cn/Article/details/giiedvqec.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.zdbjq.cn/Article/details/grnhkfplm.sHtML

cmd > out.log 2>&1
来源：http://baike.zdbjq.cn/Article/details/gdriwgbws.sHtML

[R40] 追加写日志
来源：http://www.blog.hesvh.cn/Article/details/gelctcwpr.sHtML

echo "log" >> out.log
来源：http://blog.fehbvm.com/Article/details/glrigknzd.sHtML

[R41] 丢弃输出
来源：http://baike.hesvh.cn/Article/details/ggnxyzkqx.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gsxhwheac.sHtML

[R42] 输入重定向
来源：http://m.share.hesvh.cn/Article/details/gkyhashrq.sHtML

wc -l < a.txt
来源：http://www.share.zdbjq.cn/Article/details/gyuozlyqr.sHtML

[R43] 按名字查找文件
来源：http://read.share.hesvh.cn/Article/details/gslzienci.sHtML

find . -name "*.log" -type f
来源：http://m.share.fehbvm.com/Article/details/gheeuydhc.sHtML

[R44] 按修改时间查找
来源：http://read.share.hesvh.cn/Article/details/gkofoovly.sHtML

find . -mtime -7 -type f
来源：http://www.share.zdbjq.cn/Article/details/gyedikyap.sHtML

[R45] 批量删除
来源：http://read.share.hesvh.cn/Article/details/gxekqvzwx.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/gbohfgjqr.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/gaedcffho.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fehbvm.com/Article/details/glkmkqlpv.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fehbvm.com/Article/details/gwtzrxfna.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gzyspqzry.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gccrddtiw.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gucsuldbe.sHtML

[R49] awk 带条件
来源：http://wap.fehbvm.com/Article/details/gyxrlbvzh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fehbvm.com/Article/details/grryremqb.sHtML

[R50] awk 求和
来源：http://mobile.zdbjq.cn/Article/details/gjgopcrlj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fehbvm.com/Article/details/grslniqql.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.zdbjq.cn/Article/details/gkwjjjuhn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.hesvh.cn/Article/details/gkbpoporl.sHtML

[R52] 统计行数
来源：http://blog.zdbjq.cn/Article/details/gxcgmaymw.sHtML

wc -l a.txt
来源：http://www.share.zdbjq.cn/Article/details/gumcnapum.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/gqjgaejih.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fehbvm.com/Article/details/gtwtpcvfa.sHtML

[R54] 比较两个文件
来源：http://blog.zdbjq.cn/Article/details/gyrlrbnun.sHtML

diff a.txt b.txt
来源：http://m.share.fehbvm.com/Article/details/glwgeomok.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/gceuvkxss.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/gbzwrodyb.sHtML

[R56] 远程拷贝
来源：http://www.blog.fehbvm.com/Article/details/gnvqzavqh.sHtML

scp file user@host:/path/
来源：http://www.blog.fehbvm.com/Article/details/gdcgrfjad.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/glepyoaba.sHtML

ssh user@host 'uptime'
来源：http://www.blog.zdbjq.cn/Article/details/govanmgtx.sHtML

[R58] 下载文件
来源：http://mobile.hesvh.cn/Article/details/gyrvywcle.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.hesvh.cn/Article/details/gaoitrydu.sHtML

[R59] 发 POST JSON
来源：http://wap.hesvh.cn/Article/details/gckvbdrzj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fehbvm.com/Article/details/gddqsxiuz.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gumihacsx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.zdbjq.cn/Article/details/gsayzposa.sHtML

[R61] 磁盘占用
来源：http://wap.hesvh.cn/Article/details/gqomuynak.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/ghihbvoax.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/gcodrmont.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.zdbjq.cn/Article/details/gmtgouuge.sHtML

[R63] 内存与进程
来源：http://www.share.zdbjq.cn/Article/details/giujweyta.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.zdbjq.cn/Article/details/gzgagrukn.sHtML

[R64] 结束进程
来源：http://www.blog.zdbjq.cn/Article/details/gypwstwvd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/gmmhroyss.sHtML

[R65] 查看端口占用
来源：http://www.blog.hesvh.cn/Article/details/godjzxlne.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.hesvh.cn/Article/details/gkqzftwgp.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/gtertwavy.sHtML

crontab -e;  crontab -l
来源：http://wap.zdbjq.cn/Article/details/gbrnyckmb.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.hesvh.cn/Article/details/gwuibdxjt.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/gmunbphcn.sHtML

[R68] 计算文件校验值
来源：http://mobile.hesvh.cn/Article/details/glromcbdw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.hesvh.cn/Article/details/glwemzhoj.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/grchtgvim.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/gslgmebsq.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fehbvm.com/Article/details/ghzbhlqbj.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.hesvh.cn/Article/details/ggojowios.sHtML

[R71] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/golircbta.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.hesvh.cn/Article/details/gwxrzonfw.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/gliaerlbv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gabpgazrl.sHtML

[R73] 分割大日志
来源：http://www.share.zdbjq.cn/Article/details/gmhgltebd.sHtML

split -l 1000 big.log part_
来源：http://blog.fehbvm.com/Article/details/gcatrvpak.sHtML

[R74] 批量重命名
来源：http://3g.hesvh.cn/Article/details/gidlizwuq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fehbvm.com/Article/details/gdwtnknhw.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/gjahxtahc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/gbysgqenc.sHtML

[R76] 使用临时文件
来源：http://www.blog.zdbjq.cn/Article/details/gumuhqgph.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gcbblqhum.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/ghvylqmjj.sHtML

read -rp "请输入: " ans
来源：http://baike.fehbvm.com/Article/details/gjlarbmsp.sHtML

[R78] 交互式菜单
来源：http://www.blog.fehbvm.com/Article/details/gmidryfub.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.hesvh.cn/Article/details/gtlrutcub.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/gmbucennn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/gzqpcgpsv.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/gxqfpuihx.sHtML

time ./run.sh
来源：http://baike.fehbvm.com/Article/details/gltbxpdbw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gsglipzws.sHtML

S. C / C++ 专题
来源：http://mobile.fehbvm.com/Article/details/gdmprvfcd.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gruumwfwm.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/gwkaqdnsz.sHtML

#include <stdio.h>
来源：http://read.share.fehbvm.com/Article/details/gtjsgkkbe.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.hesvh.cn/Article/details/gsqjwjssi.sHtML

[S02] C：变量与格式化输出
来源：http://wap.zdbjq.cn/Article/details/gxwouxzxf.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fehbvm.com/Article/details/gbbkjgijw.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/gziinlflb.sHtML

int x; scanf("%d", &x);
来源：http://blog.hesvh.cn/Article/details/gmvbkgngn.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/gahllusgx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.zdbjq.cn/Article/details/gyhzrkvlf.sHtML

[S05] C：字符串长度
来源：http://wap.zdbjq.cn/Article/details/gdzvjovby.sHtML

strlen(s)
来源：http://www.blog.zdbjq.cn/Article/details/gotrehaid.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/ghisisihf.sHtML

strcmp(a, b) == 0
来源：http://www.blog.zdbjq.cn/Article/details/gvsqpyuwg.sHtML

[S07] C：数组遍历求和
来源：http://m.share.hesvh.cn/Article/details/gldbeulin.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/gkwlwppkt.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.zdbjq.cn/Article/details/gbadbafqf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/gpgxsgxsv.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/gtoauipxw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/gogmfdkvy.sHtML

[S10] C：指针与解引用
来源：http://m.share.zdbjq.cn/Article/details/gdeuskzod.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/gsizycztg.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gvczcwipa.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/gpyatgkyl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.hesvh.cn/Article/details/grmmeyjvw.sHtML

fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gdpklovlr.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/gupmnzowc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.hesvh.cn/Article/details/gnfpqmxvz.sHtML

[S13] C：宏定义
来源：http://baike.fehbvm.com/Article/details/gdckmsdab.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/gasoziira.sHtML

[S14] C：枚举
来源：http://mobile.hesvh.cn/Article/details/gmyfwrpyd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.hesvh.cn/Article/details/gyialuceg.sHtML

[S15] C：类型转换
来源：http://www.blog.fehbvm.com/Article/details/gxidogdga.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/gmoghuqbd.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/gsopacmbe.sHtML

x |= (1 << 3);
来源：http://www.share.fehbvm.com/Article/details/gurewpuol.sHtML

[S17] C：安全拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gdsdjocit.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/gcfvialky.sHtML

[S18] C：命令行参数
来源：http://read.share.fehbvm.com/Article/details/gfkacjwrn.sHtML

int main(int argc, char **argv)
来源：http://3g.zdbjq.cn/Article/details/goqyhphnx.sHtML

[S19] C：快速排序
来源：http://m.share.fehbvm.com/Article/details/gicjukkxm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gctdqzthl.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/guciecxgv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gblfmpaem.sHtML

[S21] C：字符类别判断
来源：http://m.share.zdbjq.cn/Article/details/grknpvfsx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.zdbjq.cn/Article/details/goblikakh.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gvobtvqbo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fehbvm.com/Article/details/gprabqsfb.sHtML

[S23] C：随机数
来源：http://blog.zdbjq.cn/Article/details/ggowrdlhh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/ggaazuowh.sHtML

[S24] C：获取本地时间
来源：http://wap.fehbvm.com/Article/details/gohiqgkqg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fehbvm.com/Article/details/gkvgnkmnz.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/gqwjskvza.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/gpusaevew.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/gxjjfxviw.sHtML

memset(a, 0, sizeof a);
来源：http://baike.zdbjq.cn/Article/details/grcdacyue.sHtML

[S27] C：定义常量
来源：http://wap.hesvh.cn/Article/details/gmfhgcxbw.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gquxakcab.sHtML

[S28] C：静态变量
来源：http://mobile.zdbjq.cn/Article/details/gsxhvrqfg.sHtML

static int counter = 0;
来源：http://wap.fehbvm.com/Article/details/gwigcofnn.sHtML

[S29] C：变参函数
来源：http://m.share.fehbvm.com/Article/details/gqbxbnseo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.zdbjq.cn/Article/details/gqgyelqbj.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/gqlztlixl.sHtML

#ifndef X_H
来源：http://blog.hesvh.cn/Article/details/glqhplbdc.sHtML

#define X_H
来源：http://read.share.hesvh.cn/Article/details/gvvjfccsp.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/gvpgxuzth.sHtML

[S31] C++：Hello World
来源：http://blog.zdbjq.cn/Article/details/gkvsurvdf.sHtML

#include <iostream>
来源：http://mobile.fehbvm.com/Article/details/glwnqsdxl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fehbvm.com/Article/details/guluxqeoo.sHtML

[S32] C++：字符串
来源：http://www.m.share.hesvh.cn/Article/details/gfmkturyb.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/gdizvuwwf.sHtML

[S33] C++：vector 增删
来源：http://blog.fehbvm.com/Article/details/gtulvzxpv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fehbvm.com/Article/details/gixqhqpjs.sHtML

[S34] C++：遍历 vector
来源：http://3g.zdbjq.cn/Article/details/gjwpfbrkr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fehbvm.com/Article/details/gagsnxlbm.sHtML

[S35] C++：map
来源：http://www.share.fehbvm.com/Article/details/gjhndafdy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gplbmiktd.sHtML

[S36] C++：unordered_map
来源：http://www.share.fehbvm.com/Article/details/gyrxaxrvj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/geqjxwoal.sHtML


<!-- 参考信息 -->