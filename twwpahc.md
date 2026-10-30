代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.hesvh.cn/Article/details/gnqeqpywe.sHtML

[Q75] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gaokczywz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fehbvm.com/Article/details/grzovhjpn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.zdbjq.cn/Article/details/gmguelreq.sHtML

[Q76] 按天统计
来源：http://www.blog.hesvh.cn/Article/details/gkcifzovj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fehbvm.com/Article/details/gmoczdfll.sHtML

[Q77] 时间加减
来源：http://read.share.hesvh.cn/Article/details/gvlukuydx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fehbvm.com/Article/details/guqyubloz.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/gqfcxpoyl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.hesvh.cn/Article/details/gjmbzajzh.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/giuyayylz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.zdbjq.cn/Article/details/ggfpiflui.sHtML

[Q80] 字符串截取
来源：http://blog.fehbvm.com/Article/details/ggqbeosyp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/giynsojnh.sHtML

[Q81] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gdbcziegj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.hesvh.cn/Article/details/gqgbtjqfh.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.hesvh.cn/Article/details/gkydzhppu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gmmqzzwgo.sHtML

[Q83] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gsiytwcdr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/ggcobczkm.sHtML

[Q84] 去除首尾空格
来源：http://wap.fehbvm.com/Article/details/gzfkwuhws.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gsuedcyoo.sHtML

[Q85] 数值取整
来源：http://mobile.fehbvm.com/Article/details/gfblkkgnp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.hesvh.cn/Article/details/ghbuxpssj.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.hesvh.cn/Article/details/gjjlzevgy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fehbvm.com/Article/details/garcugkri.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.zdbjq.cn/Article/details/gqfzyxknk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.zdbjq.cn/Article/details/gmveefcho.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.zdbjq.cn/Article/details/gnphigepr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fehbvm.com/Article/details/gxuqdqavg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/giulfnufw.sHtML

[Q89] 判断表是否存在
来源：http://3g.zdbjq.cn/Article/details/gcargsbvn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fehbvm.com/Article/details/goclzmagk.sHtML

[Q90] 生成序号列
来源：http://wap.hesvh.cn/Article/details/gekkytilt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.zdbjq.cn/Article/details/gpssxvovh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvzhqiwhs.sHtML

R. Bash 专题
来源：http://www.share.hesvh.cn/Article/details/gvdcfgord.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpitfzyba.sHtML

[R01] shebang 与严格模式
来源：http://www.share.hesvh.cn/Article/details/gfowctpsq.sHtML

#!/usr/bin/env bash
来源：http://blog.hesvh.cn/Article/details/ggouwheob.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/ghjznxlis.sHtML

[R02] 变量赋值与使用
来源：http://www.share.zdbjq.cn/Article/details/gimraibmv.sHtML

name="Tom"; echo "$name"
来源：http://m.share.zdbjq.cn/Article/details/gxcoufxzo.sHtML

[R03] 只读变量
来源：http://mobile.fehbvm.com/Article/details/gwebxtogh.sHtML

readonly PI=3.14
来源：http://m.share.hesvh.cn/Article/details/gpnaftpai.sHtML

[R04] 位置参数
来源：http://www.blog.hesvh.cn/Article/details/gwreuugfy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fehbvm.com/Article/details/gavljdlzu.sHtML

[R05] 参数默认值
来源：http://www.share.zdbjq.cn/Article/details/gsbmuhrfm.sHtML

name="${1:-default}"
来源：http://www.blog.zdbjq.cn/Article/details/grldgavwk.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/gvjxcdbzm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/goywevant.sHtML

[R07] if 判断文件
来源：http://mobile.zdbjq.cn/Article/details/grepwvwcw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fehbvm.com/Article/details/grqzitola.sHtML

[R08] 数值比较
来源：http://wap.fehbvm.com/Article/details/grudfdaal.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fehbvm.com/Article/details/geazkywum.sHtML

[R09] 字符串比较
来源：http://m.share.zdbjq.cn/Article/details/guhcqkfdm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.zdbjq.cn/Article/details/glxpybvhp.sHtML

[R10] 正则匹配
来源：http://wap.hesvh.cn/Article/details/gooqtsrfr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.hesvh.cn/Article/details/gxlncawie.sHtML

[R11] case 多分支
来源：http://m.share.hesvh.cn/Article/details/gtjlcuwia.sHtML

case "$1" in
来源：http://read.share.fehbvm.com/Article/details/gxpcyunaa.sHtML

start) echo "启动" ;;
来源：http://baike.fehbvm.com/Article/details/gcszsaknd.sHtML

stop)  echo "停止" ;;
来源：http://www.share.hesvh.cn/Article/details/guoawfquk.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.zdbjq.cn/Article/details/gpuxzgsvf.sHtML

esac
来源：http://3g.zdbjq.cn/Article/details/ghthqxvvr.sHtML

[R12] for 遍历文件
来源：http://blog.zdbjq.cn/Article/details/ggovalpzo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fehbvm.com/Article/details/grohvkhtu.sHtML

[R13] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gewrixpon.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gczahjjqq.sHtML

[R14] C 风格 for
来源：http://m.share.zdbjq.cn/Article/details/gfvktcqci.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gfqquqwfm.sHtML

[R15] while 逐行读文件
来源：http://3g.fehbvm.com/Article/details/gtceywami.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fehbvm.com/Article/details/gxdfwmcyj.sHtML

[R16] until 等待条件
来源：http://blog.fehbvm.com/Article/details/guydjezkh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gdeplmquz.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fehbvm.com/Article/details/gsupwgzsf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fehbvm.com/Article/details/gswywwoep.sHtML

[R18] 遍历数组
来源：http://mobile.hesvh.cn/Article/details/gxqxcauma.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fehbvm.com/Article/details/gjmzhhvgw.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/gclofkohk.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/gsudvukdn.sHtML

[R20] 关联数组（字典）
来源：http://wap.fehbvm.com/Article/details/gpamlzsgh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.hesvh.cn/Article/details/gkyupdhgv.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/ggznmcgme.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/gqgpmenry.sHtML

[R22] 截取子串
来源：http://blog.hesvh.cn/Article/details/gjgztbtzq.sHtML

echo "${s:0:5}"
来源：http://3g.hesvh.cn/Article/details/gmsfyrzkv.sHtML

[R23] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/guqovajek.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.zdbjq.cn/Article/details/goixrisbx.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gdxsbavxt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.zdbjq.cn/Article/details/gwdzyeqwz.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fehbvm.com/Article/details/gjiznedqt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fehbvm.com/Article/details/gfyasiwym.sHtML

[R26] 命令替换
来源：http://baike.fehbvm.com/Article/details/gykclrbtq.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.hesvh.cn/Article/details/gtrtmqpjf.sHtML

[R27] 算术展开
来源：http://3g.fehbvm.com/Article/details/gmtfjcetw.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.zdbjq.cn/Article/details/ghvygxrvp.sHtML

[R28] 浮点运算
来源：http://www.share.zdbjq.cn/Article/details/gntgrogyi.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fehbvm.com/Article/details/gljyzorsq.sHtML

[R29] 定义函数
来源：http://wap.hesvh.cn/Article/details/gwyrqxnlp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.zdbjq.cn/Article/details/gxjcntixe.sHtML

[R30] 函数返回状态码
来源：http://3g.hesvh.cn/Article/details/gfuojclsd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/gkkzxvtfm.sHtML

[R31] 局部变量
来源：http://www.share.zdbjq.cn/Article/details/gatifappw.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/gltpvblad.sHtML

[R32] 参数个数校验
来源：http://baike.fehbvm.com/Article/details/gvvfgipmp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gzbqjdggz.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/gseousthz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/gcxkfrxwl.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/galedxksg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gjaodznmr.sHtML

[R35] 后台执行并等待
来源：http://mobile.fehbvm.com/Article/details/gzsuksdhp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/gzxfnqfrh.sHtML

[R36] 并发执行多个任务
来源：http://baike.hesvh.cn/Article/details/gamfsnygm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fehbvm.com/Article/details/gdngxaunw.sHtML

[R37] 把输出赋给变量
来源：http://www.share.zdbjq.cn/Article/details/gbiddxdfk.sHtML

files=$(ls -1)
来源：http://m.share.fehbvm.com/Article/details/gidgxhqgj.sHtML

[R38] 管道串联
来源：http://www.share.zdbjq.cn/Article/details/gwrxodrcs.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.hesvh.cn/Article/details/gqrfyelln.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fehbvm.com/Article/details/gdlvmqnnw.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/gwyqgqnad.sHtML

[R40] 追加写日志
来源：http://baike.zdbjq.cn/Article/details/gsnwvdtbb.sHtML

echo "log" >> out.log
来源：http://wap.hesvh.cn/Article/details/gvtkobiok.sHtML

[R41] 丢弃输出
来源：http://3g.hesvh.cn/Article/details/gsuekjozk.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/gvnvzcdby.sHtML

[R42] 输入重定向
来源：http://3g.zdbjq.cn/Article/details/gbqcyzuan.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/gzemhijnm.sHtML

[R43] 按名字查找文件
来源：http://mobile.hesvh.cn/Article/details/ghhomnene.sHtML

find . -name "*.log" -type f
来源：http://mobile.hesvh.cn/Article/details/gxdkvtcgm.sHtML

[R44] 按修改时间查找
来源：http://mobile.fehbvm.com/Article/details/gfhmfnzpe.sHtML

find . -mtime -7 -type f
来源：http://baike.fehbvm.com/Article/details/gygwaotrp.sHtML

[R45] 批量删除
来源：http://wap.hesvh.cn/Article/details/gvngrkfce.sHtML

find . -name "*.tmp" -delete
来源：http://baike.zdbjq.cn/Article/details/gxuzcjfcj.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/glvyzfkxd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.zdbjq.cn/Article/details/gbpoedpvs.sHtML

[R47] sed 单行替换
来源：http://m.share.fehbvm.com/Article/details/graidzcuy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gluyascgh.sHtML

[R48] awk 取指定列
来源：http://blog.fehbvm.com/Article/details/gsifdauib.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.hesvh.cn/Article/details/gywxfnnyh.sHtML

[R49] awk 带条件
来源：http://mobile.zdbjq.cn/Article/details/gymcufgja.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fehbvm.com/Article/details/gejgayrmp.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/gazzpzwmr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gliiafbef.sHtML

[R51] 排序去重取前几
来源：http://www.share.hesvh.cn/Article/details/gnjhwqusm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fehbvm.com/Article/details/goeknawzg.sHtML

[R52] 统计行数
来源：http://www.share.zdbjq.cn/Article/details/ghjaqkzpl.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/guduamdge.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/gqpejagmr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/gfpjzlmgy.sHtML

[R54] 比较两个文件
来源：http://3g.fehbvm.com/Article/details/gkuwbmuat.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/gpfycknqz.sHtML

[R55] 压缩与解压
来源：http://blog.hesvh.cn/Article/details/gkebymqij.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.hesvh.cn/Article/details/gjsszvewn.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/gxuvsfbtl.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/gwqtibtpn.sHtML

[R57] 远程执行命令
来源：http://baike.fehbvm.com/Article/details/glgdtpokt.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fehbvm.com/Article/details/gfzyleiql.sHtML

[R58] 下载文件
来源：http://baike.fehbvm.com/Article/details/gcnbsurej.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/gtxosloqm.sHtML

[R59] 发 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gbhjzooyo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/gnphluwxl.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/giiuluesx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.zdbjq.cn/Article/details/giqinzexw.sHtML

[R61] 磁盘占用
来源：http://read.share.hesvh.cn/Article/details/glagomchi.sHtML

df -h;  du -sh *
来源：http://www.blog.hesvh.cn/Article/details/gwoctbghz.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.hesvh.cn/Article/details/gveqywfpj.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fehbvm.com/Article/details/gwfeyuodw.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/guhsgrccx.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.zdbjq.cn/Article/details/grbwlzgbd.sHtML

[R64] 结束进程
来源：http://www.m.share.zdbjq.cn/Article/details/gbmvdmokx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fehbvm.com/Article/details/gxltgjnxd.sHtML

[R65] 查看端口占用
来源：http://blog.zdbjq.cn/Article/details/gznnjaumv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fehbvm.com/Article/details/gyyipziym.sHtML

[R66] 定时任务
来源：http://read.share.hesvh.cn/Article/details/gdmvrwjbg.sHtML

crontab -e;  crontab -l
来源：http://wap.fehbvm.com/Article/details/gjfklweou.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.zdbjq.cn/Article/details/gzbixgddo.sHtML

openssl rand -hex 16
来源：http://www.m.share.hesvh.cn/Article/details/gptlbvzvj.sHtML

[R68] 计算文件校验值
来源：http://blog.hesvh.cn/Article/details/ghqraqrgn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.hesvh.cn/Article/details/gbptixmkm.sHtML

[R69] 生成随机密码
来源：http://mobile.fehbvm.com/Article/details/gtbyrskqt.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fehbvm.com/Article/details/gzhitxhqv.sHtML

[R70] 时间戳与互转
来源：http://read.share.fehbvm.com/Article/details/ghzyzgbhf.sHtML

date +%s;  date -d @1700000000
来源：http://blog.hesvh.cn/Article/details/gthifivlv.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gxqnfbhmm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fehbvm.com/Article/details/gcvzfoybk.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.zdbjq.cn/Article/details/gaberdwae.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gvodgxqai.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/gokekoley.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fehbvm.com/Article/details/gpxilulbt.sHtML

[R74] 批量重命名
来源：http://www.share.fehbvm.com/Article/details/gimnnihqt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.zdbjq.cn/Article/details/gagfjysbb.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/gbtahtrez.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fehbvm.com/Article/details/gomffujcx.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fehbvm.com/Article/details/gaumtsapw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gujjwutxr.sHtML

[R77] 读取用户输入
来源：http://www.share.fehbvm.com/Article/details/goovftuev.sHtML

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/gtvswvofe.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/gthafaitv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/gfinjpndw.sHtML

[R79] 解析命令行选项
来源：http://wap.hesvh.cn/Article/details/gradwnxte.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.hesvh.cn/Article/details/gawiqxgna.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.hesvh.cn/Article/details/gqdwfwrae.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/glscbnwhi.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gagewqtcq.sHtML

S. C / C++ 专题
来源：http://www.share.hesvh.cn/Article/details/gvneiuegk.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghhqzdfww.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gqdgtjgld.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/guyarqvui.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.zdbjq.cn/Article/details/gfpcxqjqy.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/gtqrbxwjd.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/gzleegagf.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gshqiofbo.sHtML

int x; scanf("%d", &x);
来源：http://mobile.zdbjq.cn/Article/details/grzqkunpf.sHtML

[S04] C：字符串复制
来源：http://www.share.zdbjq.cn/Article/details/gaxayvzav.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gkrtiojdk.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/gqqkkeyyd.sHtML

strlen(s)
来源：http://mobile.fehbvm.com/Article/details/gxtefwfft.sHtML

[S06] C：字符串比较
来源：http://3g.fehbvm.com/Article/details/gjryuxspk.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/gkxiwwzcg.sHtML

[S07] C：数组遍历求和
来源：http://m.share.hesvh.cn/Article/details/gkoquzdof.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.zdbjq.cn/Article/details/ginujyhcd.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.hesvh.cn/Article/details/gnqczcdzg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/gipbxvvyv.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/gwpoxjisb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.hesvh.cn/Article/details/ghzrmwlhu.sHtML

[S10] C：指针与解引用
来源：http://read.share.fehbvm.com/Article/details/gsxuryqer.sHtML

int *p = &a;  *p = 5;
来源：http://blog.hesvh.cn/Article/details/gpbzyfqfg.sHtML

[S11] C：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gpabwlbyl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/grpobyjgw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gjgqtbjhb.sHtML

fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gmoxnpkyl.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/givsraazx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/goorqchcq.sHtML

[S13] C：宏定义
来源：http://baike.hesvh.cn/Article/details/gsqmvdefv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fehbvm.com/Article/details/gabmquhqi.sHtML

[S14] C：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gunwkuvgo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/gonbinitx.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/gwordpnwn.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/grofbjjcu.sHtML

[S16] C：位操作置位
来源：http://3g.fehbvm.com/Article/details/gulmpacjz.sHtML

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/gutnnnbhy.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gholvzwom.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fehbvm.com/Article/details/gdckovmid.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gbfxhfnkx.sHtML

int main(int argc, char **argv)
来源：http://3g.fehbvm.com/Article/details/gxbdqtfqa.sHtML

[S19] C：快速排序
来源：http://www.blog.zdbjq.cn/Article/details/gbvtiwrpt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/ggecuelbk.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/gunolffjs.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gxgkpavpi.sHtML

[S21] C：字符类别判断
来源：http://blog.zdbjq.cn/Article/details/gxkirgjes.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.zdbjq.cn/Article/details/ghfowyhuu.sHtML

[S22] C：字符串转数字
来源：http://3g.fehbvm.com/Article/details/gvkeozina.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.zdbjq.cn/Article/details/grfuasasy.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/gpwpduyiu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.hesvh.cn/Article/details/gvjoefmbo.sHtML

[S24] C：获取本地时间
来源：http://wap.fehbvm.com/Article/details/gikwqchtk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.zdbjq.cn/Article/details/gqqmnnban.sHtML

[S25] C：内存拷贝
来源：http://baike.fehbvm.com/Article/details/gesviurmr.sHtML

memcpy(dst, src, n);
来源：http://3g.zdbjq.cn/Article/details/gxfopybwp.sHtML

[S26] C：内存清零
来源：http://mobile.hesvh.cn/Article/details/gqckzjoow.sHtML

memset(a, 0, sizeof a);
来源：http://baike.zdbjq.cn/Article/details/gwivuljvg.sHtML

[S27] C：定义常量
来源：http://read.share.hesvh.cn/Article/details/gquqbgmsf.sHtML

const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gquedjmvj.sHtML

[S28] C：静态变量
来源：http://read.share.hesvh.cn/Article/details/gugbnspbs.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/gpchatpqq.sHtML

[S29] C：变参函数
来源：http://m.share.fehbvm.com/Article/details/goqkdqvlo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.zdbjq.cn/Article/details/gtniorubh.sHtML

[S30] C：头文件保护
来源：http://3g.hesvh.cn/Article/details/gabqwarqn.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/gadahffmn.sHtML

#define X_H
来源：http://www.blog.hesvh.cn/Article/details/gwmcplkep.sHtML

#endif
来源：http://www.blog.fehbvm.com/Article/details/grzuxzzpb.sHtML

[S31] C++：Hello World
来源：http://blog.hesvh.cn/Article/details/gwhkpkpgd.sHtML

#include <iostream>
来源：http://3g.hesvh.cn/Article/details/gsmzopmwq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.hesvh.cn/Article/details/gtblorewp.sHtML

[S32] C++：字符串
来源：http://blog.hesvh.cn/Article/details/gvauzyonr.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fehbvm.com/Article/details/grkgvbdvx.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/gcudnjpyv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.hesvh.cn/Article/details/gjfymyymt.sHtML

[S34] C++：遍历 vector
来源：http://baike.fehbvm.com/Article/details/glpjzgqbd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/gynjzcimi.sHtML

[S35] C++：map
来源：http://blog.fehbvm.com/Article/details/glzgtgvey.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gvycobfsp.sHtML

[S36] C++：unordered_map
来源：http://mobile.fehbvm.com/Article/details/gjrtzopza.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gywjvuutp.sHtML

[S37] C++：set
来源：http://www.share.fehbvm.com/Article/details/gsoxyzjke.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fehbvm.com/Article/details/giphpmhja.sHtML

[S38] C++：排序
来源：http://www.share.hesvh.cn/Article/details/gboqrvger.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.hesvh.cn/Article/details/gpnfavfsm.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fehbvm.com/Article/details/gupartumr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.hesvh.cn/Article/details/gwjtkobme.sHtML

[S40] C++：查找元素
来源：http://m.share.hesvh.cn/Article/details/gwngmjwpb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/gktltvsgo.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fehbvm.com/Article/details/gxcikcvdu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fehbvm.com/Article/details/gqgjrhhfu.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.zdbjq.cn/Article/details/gnfntbsch.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/gphqbulmj.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gkilbpxpg.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/gcgjphgfy.sHtML

[S44] C++：引用传参
来源：http://baike.fehbvm.com/Article/details/gwrlfothn.sHtML

void inc(int &x) { ++x; }
来源：http://3g.zdbjq.cn/Article/details/gcawozfqk.sHtML


<!-- 参考信息 -->