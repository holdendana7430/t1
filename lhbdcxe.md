代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.hesvh.cn/Article/details/gxctwhaxc.sHtML

[Q75] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gjjdlzqfb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gxkxnzzfe.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.hesvh.cn/Article/details/gksmrzfdh.sHtML

[Q76] 按天统计
来源：http://3g.fehbvm.com/Article/details/gpoersgsu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.hesvh.cn/Article/details/gqvepoueg.sHtML

[Q77] 时间加减
来源：http://wap.fehbvm.com/Article/details/gjsxdimzx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fehbvm.com/Article/details/gsegnjizw.sHtML

[Q78] 当前时间
来源：http://wap.hesvh.cn/Article/details/gtcdttmcm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.hesvh.cn/Article/details/ginkgbuwa.sHtML

[Q79] 字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gnvzkogbj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fehbvm.com/Article/details/gufqjzvbe.sHtML

[Q80] 字符串截取
来源：http://3g.zdbjq.cn/Article/details/gndexvhhv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gdcmwpqza.sHtML

[Q81] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/giaetggfw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.hesvh.cn/Article/details/gfeanqlgk.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fehbvm.com/Article/details/gophkspbo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gytdrrmfm.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gvmztxcrt.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/ggkuehttu.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fehbvm.com/Article/details/gaulgqiue.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gskuhhzid.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/gzhihahzp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.hesvh.cn/Article/details/gqjuznjfi.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.hesvh.cn/Article/details/gbswzpdee.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.zdbjq.cn/Article/details/gmggpdigw.sHtML

[Q87] JSON 字段做条件
来源：http://wap.hesvh.cn/Article/details/gkszbgpae.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fehbvm.com/Article/details/grpajnvlj.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/gnympjyiw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fehbvm.com/Article/details/gvuusrjbt.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.zdbjq.cn/Article/details/ghsarapye.sHtML

[Q89] 判断表是否存在
来源：http://m.share.hesvh.cn/Article/details/gzhpiiczu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.hesvh.cn/Article/details/ghchmogvr.sHtML

[Q90] 生成序号列
来源：http://www.share.fehbvm.com/Article/details/gauftkode.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.hesvh.cn/Article/details/gkgdebfql.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmmlkkhzi.sHtML

R. Bash 专题
来源：http://www.blog.fehbvm.com/Article/details/gxlgezyuw.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gniddcaqr.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/gqoyqgxdh.sHtML

#!/usr/bin/env bash
来源：http://wap.fehbvm.com/Article/details/gayzkjemw.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/grvujgqks.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fehbvm.com/Article/details/ggzcyqfkp.sHtML

name="Tom"; echo "$name"
来源：http://blog.hesvh.cn/Article/details/gevrlwvhe.sHtML

[R03] 只读变量
来源：http://m.share.fehbvm.com/Article/details/gdjftktuw.sHtML

readonly PI=3.14
来源：http://m.share.zdbjq.cn/Article/details/gsbpiibze.sHtML

[R04] 位置参数
来源：http://www.share.fehbvm.com/Article/details/gxspdrxie.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.zdbjq.cn/Article/details/grxtxvyyr.sHtML

[R05] 参数默认值
来源：http://blog.hesvh.cn/Article/details/goawqkwsl.sHtML

name="${1:-default}"
来源：http://read.share.hesvh.cn/Article/details/gcgmfmpvi.sHtML

[R06] 判断命令是否存在
来源：http://www.share.hesvh.cn/Article/details/gbraczoog.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gxhcdopys.sHtML

[R07] if 判断文件
来源：http://read.share.fehbvm.com/Article/details/gnoceizmy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fehbvm.com/Article/details/gnngivqqj.sHtML

[R08] 数值比较
来源：http://www.share.hesvh.cn/Article/details/gknfydjef.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gwynheogy.sHtML

[R09] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/gpveuxnpf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/guanzozwf.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/gmzxkvdxc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.zdbjq.cn/Article/details/guqydrkvx.sHtML

[R11] case 多分支
来源：http://blog.hesvh.cn/Article/details/gfgxcgtlw.sHtML

case "$1" in
来源：http://blog.hesvh.cn/Article/details/grudpuest.sHtML

start) echo "启动" ;;
来源：http://read.share.fehbvm.com/Article/details/gegmrkang.sHtML

stop)  echo "停止" ;;
来源：http://baike.zdbjq.cn/Article/details/gwzyzudta.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fehbvm.com/Article/details/gvgyfxamd.sHtML

esac
来源：http://baike.hesvh.cn/Article/details/gjirfllnh.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/gynffizhq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fehbvm.com/Article/details/goyfxlfgg.sHtML

[R13] for 计数循环
来源：http://m.share.fehbvm.com/Article/details/gaiyhgaoq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gtdkpjkba.sHtML

[R14] C 风格 for
来源：http://blog.hesvh.cn/Article/details/gsqkyfilk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gdugczwdg.sHtML

[R15] while 逐行读文件
来源：http://3g.fehbvm.com/Article/details/gadigxtqv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fehbvm.com/Article/details/gkevdmuwv.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/gkoepewmy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gortcvjkj.sHtML

[R17] 数组定义与取值
来源：http://3g.fehbvm.com/Article/details/gnmxwakik.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fehbvm.com/Article/details/gsurlqpni.sHtML

[R18] 遍历数组
来源：http://www.blog.fehbvm.com/Article/details/glppvxrkp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.hesvh.cn/Article/details/gocdcizdg.sHtML

[R19] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/giborwigz.sHtML

echo "${#arr[@]}"
来源：http://www.blog.zdbjq.cn/Article/details/gyxaeghyk.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.hesvh.cn/Article/details/gazvcsbcn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gaftbnfbi.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gvwbdpobq.sHtML

echo "${#s}"
来源：http://www.blog.hesvh.cn/Article/details/gpundbsvb.sHtML

[R22] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gzrpamjqi.sHtML

echo "${s:0:5}"
来源：http://wap.fehbvm.com/Article/details/gqrnvolis.sHtML

[R23] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gjxqfuote.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.zdbjq.cn/Article/details/giqfgnqtp.sHtML

[R24] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gwuathdsk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.hesvh.cn/Article/details/gijlzmubz.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gtchezcfm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.zdbjq.cn/Article/details/gndvbjjzb.sHtML

[R26] 命令替换
来源：http://www.m.share.hesvh.cn/Article/details/gqhnqbjvj.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.zdbjq.cn/Article/details/grejshwnt.sHtML

[R27] 算术展开
来源：http://www.share.hesvh.cn/Article/details/gbraoknkr.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.zdbjq.cn/Article/details/grjlkshxa.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/gggbncnoc.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/gunzgholw.sHtML

[R29] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gxjrqpxjd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/gpzroqgfj.sHtML

[R30] 函数返回状态码
来源：http://3g.hesvh.cn/Article/details/gqbfcrkhs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fehbvm.com/Article/details/gtlukawsc.sHtML

[R31] 局部变量
来源：http://www.share.zdbjq.cn/Article/details/ggapgohpj.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fehbvm.com/Article/details/gkfonfdme.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/gbbgefdru.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gdciscbkl.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.zdbjq.cn/Article/details/gwguwuvvy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fehbvm.com/Article/details/girvkoikr.sHtML

[R34] 退出时清理
来源：http://mobile.fehbvm.com/Article/details/gxnwvcixs.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gjioxdhrc.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/gyqglxenr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.zdbjq.cn/Article/details/gdgxowevg.sHtML

[R36] 并发执行多个任务
来源：http://read.share.zdbjq.cn/Article/details/gkwbeluzf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fehbvm.com/Article/details/gkacxbhjc.sHtML

[R37] 把输出赋给变量
来源：http://baike.zdbjq.cn/Article/details/ggjgtbhuu.sHtML

files=$(ls -1)
来源：http://blog.zdbjq.cn/Article/details/gdicmkbye.sHtML

[R38] 管道串联
来源：http://3g.fehbvm.com/Article/details/gjnxsilts.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fehbvm.com/Article/details/gtgdajgqy.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.hesvh.cn/Article/details/gxsmvnafd.sHtML

cmd > out.log 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gztumyquh.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/gxshtfqmp.sHtML

echo "log" >> out.log
来源：http://www.share.fehbvm.com/Article/details/gbnznpibc.sHtML

[R41] 丢弃输出
来源：http://m.share.zdbjq.cn/Article/details/gebwmnsdw.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gharucrhe.sHtML

[R42] 输入重定向
来源：http://mobile.zdbjq.cn/Article/details/gaxmvofsa.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/gnonhduuz.sHtML

[R43] 按名字查找文件
来源：http://blog.hesvh.cn/Article/details/giojtvntm.sHtML

find . -name "*.log" -type f
来源：http://baike.zdbjq.cn/Article/details/ghxmzqwzc.sHtML

[R44] 按修改时间查找
来源：http://read.share.zdbjq.cn/Article/details/gluojclto.sHtML

find . -mtime -7 -type f
来源：http://www.share.fehbvm.com/Article/details/gjqvxzuyh.sHtML

[R45] 批量删除
来源：http://read.share.hesvh.cn/Article/details/gntvigqly.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.zdbjq.cn/Article/details/gkvjpuuzo.sHtML

[R46] 递归替换文件内容
来源：http://m.share.zdbjq.cn/Article/details/gayfrgfgc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fehbvm.com/Article/details/gqepdlnoa.sHtML

[R47] sed 单行替换
来源：http://m.share.hesvh.cn/Article/details/gyquxemzb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gwslzxlwz.sHtML

[R48] awk 取指定列
来源：http://read.share.fehbvm.com/Article/details/gccfyfbag.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gneyshhky.sHtML

[R49] awk 带条件
来源：http://www.share.hesvh.cn/Article/details/gltddnonw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fehbvm.com/Article/details/gnsluwioj.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/gipygfroa.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/ghsqigeow.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/gcscdqgkf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.zdbjq.cn/Article/details/ghrpxklpb.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/girdxgmsp.sHtML

wc -l a.txt
来源：http://3g.fehbvm.com/Article/details/gjkcodmjn.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fehbvm.com/Article/details/gtrzctcbz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.zdbjq.cn/Article/details/gfwpelwha.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/gnzvyjtxd.sHtML

diff a.txt b.txt
来源：http://wap.fehbvm.com/Article/details/gpbpavtrh.sHtML

[R55] 压缩与解压
来源：http://blog.hesvh.cn/Article/details/gaoqlrvvr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.zdbjq.cn/Article/details/guiscyzix.sHtML

[R56] 远程拷贝
来源：http://www.share.hesvh.cn/Article/details/gmgpelslr.sHtML

scp file user@host:/path/
来源：http://wap.hesvh.cn/Article/details/gjgmuxhqi.sHtML

[R57] 远程执行命令
来源：http://baike.hesvh.cn/Article/details/glbfpteee.sHtML

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/grgyfacmk.sHtML

[R58] 下载文件
来源：http://www.share.fehbvm.com/Article/details/gnelyfvub.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/grdwklwls.sHtML

[R59] 发 POST JSON
来源：http://m.share.hesvh.cn/Article/details/gqjvfpans.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.zdbjq.cn/Article/details/gbjztlezn.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/geqogmaxh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fehbvm.com/Article/details/gwlsdcxsy.sHtML

[R61] 磁盘占用
来源：http://mobile.zdbjq.cn/Article/details/ggsbfaatn.sHtML

df -h;  du -sh *
来源：http://www.blog.hesvh.cn/Article/details/grwxcnvcl.sHtML

[R62] 找最占空间的文件
来源：http://m.share.hesvh.cn/Article/details/ginraplsi.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.hesvh.cn/Article/details/gisvrjxep.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/gaucbdxcf.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.hesvh.cn/Article/details/gzroqrkfi.sHtML

[R64] 结束进程
来源：http://3g.zdbjq.cn/Article/details/gtmlwctgl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.hesvh.cn/Article/details/gwselxbbz.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/gjwiqebzi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.hesvh.cn/Article/details/gpjhjerra.sHtML

[R66] 定时任务
来源：http://3g.zdbjq.cn/Article/details/ghvtywbui.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/givyoyhwq.sHtML

[R67] 生成随机十六进制串
来源：http://blog.hesvh.cn/Article/details/guakyuxtq.sHtML

openssl rand -hex 16
来源：http://read.share.zdbjq.cn/Article/details/gfxcursfk.sHtML

[R68] 计算文件校验值
来源：http://mobile.zdbjq.cn/Article/details/ghadhdign.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/gqvikftoq.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/gwtjbjeby.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/gstvemxxl.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/gitxmjris.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/gctpgkoma.sHtML

[R71] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gsenuxlen.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fehbvm.com/Article/details/ghjpjysmr.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/gswvairfr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/geeikgpid.sHtML

[R73] 分割大日志
来源：http://www.m.share.zdbjq.cn/Article/details/gnhcxskbh.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fehbvm.com/Article/details/gzfgvqzki.sHtML

[R74] 批量重命名
来源：http://www.m.share.zdbjq.cn/Article/details/gdkmxmkyf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.zdbjq.cn/Article/details/gpxbueuka.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/gyrapuzxj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/gjwrmilqr.sHtML

[R76] 使用临时文件
来源：http://baike.fehbvm.com/Article/details/gizfklxii.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gyqzjgtdf.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/gyzfvuzxa.sHtML

read -rp "请输入: " ans
来源：http://m.share.fehbvm.com/Article/details/gdcmhmlgr.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/gyqzakukx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fehbvm.com/Article/details/gsemkcnso.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/gsliiigwl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fehbvm.com/Article/details/gnhvfbmsg.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/gxxynbntf.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/gytpqzypa.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzhppvrwk.sHtML

S. C / C++ 专题
来源：http://www.share.hesvh.cn/Article/details/gouwalqsa.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gpeuhacax.sHtML

[S01] C：Hello World
来源：http://m.share.fehbvm.com/Article/details/gvoqzfjeh.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/gytwhfoou.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/gbjbkjjwv.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fehbvm.com/Article/details/gplgfuppd.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.zdbjq.cn/Article/details/gaknmgmhp.sHtML

[S03] C：读入整数
来源：http://m.share.zdbjq.cn/Article/details/gefiirwge.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/gmetsivla.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/gyttbaecv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.hesvh.cn/Article/details/gigcqaawh.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gjjacuaoc.sHtML

strlen(s)
来源：http://m.share.zdbjq.cn/Article/details/grkpyayvj.sHtML

[S06] C：字符串比较
来源：http://www.share.fehbvm.com/Article/details/ggapokvlq.sHtML

strcmp(a, b) == 0
来源：http://3g.fehbvm.com/Article/details/gzzymcbdh.sHtML

[S07] C：数组遍历求和
来源：http://blog.fehbvm.com/Article/details/glbehofna.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fehbvm.com/Article/details/gojugfumh.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/gfmbcmjxc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.zdbjq.cn/Article/details/gxwjlwbvq.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.zdbjq.cn/Article/details/gzzlpcyaq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fehbvm.com/Article/details/gnlhfnzfj.sHtML

[S10] C：指针与解引用
来源：http://3g.zdbjq.cn/Article/details/gnyktpnwk.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/gwemuarey.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gonimeyce.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fehbvm.com/Article/details/gmxcalnqr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/gcjjvwjgh.sHtML

fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gjjkfazam.sHtML

[S12] C：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gwzovgrtr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/ghghgizdf.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/gzflgtrqj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.zdbjq.cn/Article/details/gpfohvcxu.sHtML

[S14] C：枚举
来源：http://mobile.hesvh.cn/Article/details/gxamzplnt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fehbvm.com/Article/details/gjwpayatt.sHtML

[S15] C：类型转换
来源：http://www.blog.fehbvm.com/Article/details/gnqjzuodt.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/gyumjjhep.sHtML

[S16] C：位操作置位
来源：http://mobile.hesvh.cn/Article/details/gtamehqmv.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/gwckfqkfj.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fehbvm.com/Article/details/glnuaciwa.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fehbvm.com/Article/details/gnagqpfte.sHtML

[S18] C：命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gksfixgkh.sHtML

int main(int argc, char **argv)
来源：http://mobile.hesvh.cn/Article/details/gdkihonym.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/gcrtuefpd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gbqqkgwns.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/glpjovhyu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gfhxheisa.sHtML

[S21] C：字符类别判断
来源：http://3g.hesvh.cn/Article/details/gwgqlxtbi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.zdbjq.cn/Article/details/gbuxowvoq.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/glxfmlpmf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.zdbjq.cn/Article/details/ghnrvtxmg.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gnyacslud.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/giwnzcymf.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/gcukiagku.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/gpohgajhy.sHtML

[S25] C：内存拷贝
来源：http://read.share.zdbjq.cn/Article/details/grgdijolz.sHtML

memcpy(dst, src, n);
来源：http://blog.zdbjq.cn/Article/details/gnmljwmcs.sHtML

[S26] C：内存清零
来源：http://baike.zdbjq.cn/Article/details/gzowffcqo.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.hesvh.cn/Article/details/guntagepk.sHtML

[S27] C：定义常量
来源：http://www.blog.fehbvm.com/Article/details/gffuzujpx.sHtML

const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gscujiqey.sHtML

[S28] C：静态变量
来源：http://www.blog.hesvh.cn/Article/details/gkjpqmaxm.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/gysyyniww.sHtML

[S29] C：变参函数
来源：http://m.share.fehbvm.com/Article/details/gpjiunhyd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fehbvm.com/Article/details/gemretaur.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/gkoxjwkmb.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/grzfwbvlo.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/gchzeacsh.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/gbejytlby.sHtML

[S31] C++：Hello World
来源：http://blog.fehbvm.com/Article/details/gyjavkbob.sHtML

#include <iostream>
来源：http://wap.fehbvm.com/Article/details/gfmqhgrci.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.hesvh.cn/Article/details/gukggbsre.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gksaerswr.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/guznpxitw.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/glqorzmhg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/gqqfeckzw.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/ghifadhtj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fehbvm.com/Article/details/gbibsfaux.sHtML

[S35] C++：map
来源：http://blog.fehbvm.com/Article/details/ghmzbpkuk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gsaroqvgc.sHtML

[S36] C++：unordered_map
来源：http://wap.hesvh.cn/Article/details/guviwiywr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gksreabwo.sHtML

[S37] C++：set
来源：http://3g.zdbjq.cn/Article/details/gwfubwohu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fehbvm.com/Article/details/gwlcxfqog.sHtML

[S38] C++：排序
来源：http://mobile.zdbjq.cn/Article/details/gdgdnkadz.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gbzqvsees.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.zdbjq.cn/Article/details/gurmyesru.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.zdbjq.cn/Article/details/grpvgvhhd.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/gthbojznw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.hesvh.cn/Article/details/giwrupkua.sHtML

[S41] C++：类与构造函数
来源：http://3g.fehbvm.com/Article/details/gjuvqsyya.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/gjabfbwvz.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/gieeskgdo.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.zdbjq.cn/Article/details/gfvrmhjvn.sHtML

[S43] C++：智能指针
来源：http://m.share.zdbjq.cn/Article/details/gktoygnbf.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fehbvm.com/Article/details/gcjroifpw.sHtML

[S44] C++：引用传参
来源：http://baike.zdbjq.cn/Article/details/gxkkbsoqx.sHtML

void inc(int &x) { ++x; }
来源：http://wap.hesvh.cn/Article/details/gmsleeokn.sHtML


<!-- 参考信息 -->