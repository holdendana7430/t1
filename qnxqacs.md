代发 wailian999

SHOW INDEX FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gouldwrtm.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/gchspjzbm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gzktzhkxg.sHtML

[Q74] 强制使用索引
来源：http://baike.fanxiaobao.xyz/Article/details/gginenvgz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fanxiaobao.xyz/Article/details/guekzsvep.sHtML

[Q75] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gsijspoxo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gkxolwmck.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fanxiaobao.xyz/Article/details/gehtuebqr.sHtML

[Q76] 按天统计
来源：http://baike.fanxiaobao.xyz/Article/details/gcasxlmao.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdrfxmzy.sHtML

[Q77] 时间加减
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbuqericl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfytsxyd.sHtML

[Q78] 当前时间
来源：http://baike.fanxiaobao.xyz/Article/details/gmbqpthpu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fanxiaobao.xyz/Article/details/gwaheykml.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldcgycaf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjafxzsi.sHtML

[Q80] 字符串截取
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqdtustp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlkidugm.sHtML

[Q81] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gxprhcpkh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwhqjcyn.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fanxiaobao.xyz/Article/details/grfmgglxi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/ghvcgebxv.sHtML

[Q83] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnjstzri.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlqvqwjb.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fanxiaobao.xyz/Article/details/gygxwfziz.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtezwcvod.sHtML

[Q85] 数值取整
来源：http://read.share.fanxiaobao.xyz/Article/details/ghielcqoz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fanxiaobao.xyz/Article/details/gquvrlifh.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpwlzdtk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fanxiaobao.xyz/Article/details/gdoozcmay.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjusazsud.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fanxiaobao.xyz/Article/details/geclylcvr.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/gkauvawrm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/gqqkqspbn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvuakbio.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcvmjery.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/grskczggq.sHtML

[Q90] 生成序号列
来源：http://wap.fanxiaobao.xyz/Article/details/gvsgdacqo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fanxiaobao.xyz/Article/details/gavjclmkm.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmtfktyy.sHtML

R. Bash 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gywrurkmq.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbicicvm.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/gdesbxyqs.sHtML

#!/usr/bin/env bash
来源：http://3g.fanxiaobao.xyz/Article/details/gcghxgtzx.sHtML

set -euo pipefail
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzpqsftv.sHtML

[R02] 变量赋值与使用
来源：http://blog.fanxiaobao.xyz/Article/details/gvrhmefvi.sHtML

name="Tom"; echo "$name"
来源：http://wap.fanxiaobao.xyz/Article/details/gdoztjtqu.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gumolesuq.sHtML

readonly PI=3.14
来源：http://3g.fanxiaobao.xyz/Article/details/gwnkmwbvr.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/gfktqosay.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fanxiaobao.xyz/Article/details/glldfphby.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gnuxcbnnc.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/gcqffaivu.sHtML

[R06] 判断命令是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gexcjcyqz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfoymbnqa.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdjtjqza.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/goexhxvvj.sHtML

[R08] 数值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxnsebcm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gcckiqyee.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzyqlcmrr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqeuohab.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwifjxbb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gvmtgsznb.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/gevbxrzcw.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjjrnovm.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gxxueuupx.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gexbghufq.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtyuwapnm.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdkgwykj.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gqgrerozc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwllwyip.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gufolxvuc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpiachcf.sHtML

[R14] C 风格 for
来源：http://read.share.fanxiaobao.xyz/Article/details/gexraviko.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gnrxsvdmq.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gkuljxycu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gincwwwch.sHtML

[R16] until 等待条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gawlbiftb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzrnhatb.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/gjfyjuifh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/guggrpurr.sHtML

[R18] 遍历数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgudiiuf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gmywtzrts.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gnttdxzbu.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gbwbutvtb.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/gwixuvpps.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcyluoibj.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gsqtfddom.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbvytmpl.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqtduebk.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/goqpfpiyz.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gjpprrkfz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/godlizaup.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/glijbboet.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgsaiauz.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaenjmbdo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/gmpoduoqg.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gfvlxgqex.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkhaeopv.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnfzfhlj.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmtpeffw.sHtML

[R28] 浮点运算
来源：http://blog.fanxiaobao.xyz/Article/details/gqyxgbsqt.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggyeszrru.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gholxniev.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/gbmiutotd.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/ggsxhigbk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvplsxzvt.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvrvgibl.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjlajzbkz.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdpekbua.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxnejaeyp.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gpaezifbw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/gyvyptiwr.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/gtpnctncd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmymvzrxc.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmmauhtn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaweguqfm.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpzpgebf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/gqqraiaat.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwurfyac.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrlyknnb.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqulknjfa.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvyuigcv.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgxrkyyo.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrnhlgnd.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gppwgcwwj.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/geztszvck.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gcwfextue.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gtimckywp.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwnppglo.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfwltual.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjjusotk.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gdurosokf.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gxinpogfa.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gwdkwsqrr.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gyivfappw.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnsvwwpi.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/glnevgtco.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gbwnmexwx.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/girgdirtt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gfsqhpgvz.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/ghdzrpkwe.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gejvtprmq.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gookpipky.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gnnpgvjok.sHtML

[R50] awk 求和
来源：http://3g.fanxiaobao.xyz/Article/details/gqumjxswo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/ghegavsqr.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gteckztui.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gslhaxiwc.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gtudkmcud.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtoommnc.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gzifnxylv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtynahkj.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gbhldijct.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gexowwwaw.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/gfrfjcsgk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gpahzrjmy.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbpwghqa.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/gscqzhibg.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnqcwrtg.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/glzlapveo.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gbqmiptiv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhxrrkhm.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcpruknp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzautuof.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gzdvqvotp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrpsfipf.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gffetkuam.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/gsaflxetg.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdbwcwim.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqlajfiw.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gwentjpea.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gycuzaiwv.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gxikgludp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/godxztnnt.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gavhsvsla.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gihdxkxxo.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/ganwppnkx.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gljkwspyq.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gzakrjemw.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gozkhovej.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzeroubg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gumnrnpec.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/geggtrton.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqllvhvkx.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gqsyxbgsn.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gzimqihyn.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gfqvtaofo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gspovffkt.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gxvvoebdi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnvdytke.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/grhtjjght.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gedsmmvcu.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimogrffs.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebdqqrdh.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gsewkxiuj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gusvchjsu.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzaelyyxu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gzshohmid.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/glqpfrrma.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/gzekupnqh.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gsumizjor.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlcsqwrx.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gcaccymsu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/grnpzmcls.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gflrreuuu.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/gzqzoinwc.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gygharbkd.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/ghuydxpip.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gnkyaslie.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbtpdcbp.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gxuvrjclp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gslmrydar.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/grknszvth.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxakyydiu.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gdyuprzwo.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/gzgmozmxh.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdbiyrah.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmxkoedg.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/ggwvjdlxo.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazrhkadc.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/goajtdzfm.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjpzdrhe.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gkusxvrpe.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gfjpqlguz.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gwacnvgxt.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbcybtvy.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gijkpschl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gbjsrhkbf.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbozppov.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgrwwifv.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gqrekhfye.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/gbruslivy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmuprigd.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtxboesq.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gfbchlbur.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtafyiwed.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goejvtyrj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/grztkbhri.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdtmctmd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/gvynhdfvb.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gxamzhzob.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gltsftiof.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gkdjezvfl.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghijmckfi.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gkqkmngba.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/gysfymsfb.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwtxslcp.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gubigsexr.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbtxdbyu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gykflokfv.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmndnyqf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/guoqzecuv.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gaihrqblp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcckfyss.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gwptjvdwb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/ggepqvmnm.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gmohfpyjb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqjgiehw.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gonrihcfh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gochnnpkr.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gajpxouxx.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbxmfhgz.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/grijekfus.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrpvohty.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gmjowfebd.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbugiweh.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrhfjyro.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/glbnxlzun.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujpchtfm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gihxxfers.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrcyocem.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/ggayffjil.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqabvezh.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gknhoapum.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gugqewiuh.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdyhapwn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopkqjbku.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gfozltswf.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwryyagvy.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gftarqrlo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/giukyuhvy.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gbnqmubyx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdwdweviu.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/glwjuayrm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gptajburu.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gqnqvzcxn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gmakbgunc.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/gombyjhob.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpagycyt.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gtxzojjgf.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqipjwmf.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwctgask.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/gzbuzewit.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gtvjvtlrx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhpngitv.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gznlhsbyl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galgigvlm.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gieoaobog.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjncraet.sHtML


<!-- 参考信息 -->