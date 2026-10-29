代发 wailian999

[Q82] 字符长度与字节长度
来源：http://www.share.hesvh.cn/Article/details/gtmksppxy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gbwvnzuka.sHtML

[Q83] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/givbivssd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/glbmbnbis.sHtML

[Q84] 去除首尾空格
来源：http://www.share.hesvh.cn/Article/details/gudnvlbnj.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gebtplqxm.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/gujwpbalv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.zdbjq.cn/Article/details/gussocoid.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fehbvm.com/Article/details/ghngauajm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/ghjfzsagd.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.zdbjq.cn/Article/details/gsjdytelf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fehbvm.com/Article/details/gmndajppu.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fehbvm.com/Article/details/grjmejrjv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/gipiaddxq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fehbvm.com/Article/details/gsmasmqbn.sHtML

[Q89] 判断表是否存在
来源：http://baike.fehbvm.com/Article/details/gxskfjiry.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.hesvh.cn/Article/details/gnbjvfzyj.sHtML

[Q90] 生成序号列
来源：http://mobile.fehbvm.com/Article/details/griljcczg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.hesvh.cn/Article/details/gjyqbfdld.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gofkalwod.sHtML

R. Bash 专题
来源：http://read.share.hesvh.cn/Article/details/ggmrlqjap.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gduxwikxp.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/gyxzlftcd.sHtML

#!/usr/bin/env bash
来源：http://3g.fehbvm.com/Article/details/gshaydval.sHtML

set -euo pipefail
来源：http://mobile.hesvh.cn/Article/details/gzpnkhkly.sHtML

[R02] 变量赋值与使用
来源：http://www.share.zdbjq.cn/Article/details/gvmgfcaof.sHtML

name="Tom"; echo "$name"
来源：http://baike.hesvh.cn/Article/details/glkqeykbz.sHtML

[R03] 只读变量
来源：http://blog.fehbvm.com/Article/details/gcvzidopg.sHtML

readonly PI=3.14
来源：http://www.m.share.zdbjq.cn/Article/details/grgtwsirr.sHtML

[R04] 位置参数
来源：http://www.m.share.hesvh.cn/Article/details/guqwjfhmk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/gdtmxxmhb.sHtML

[R05] 参数默认值
来源：http://m.share.fehbvm.com/Article/details/golfazgru.sHtML

name="${1:-default}"
来源：http://3g.zdbjq.cn/Article/details/gcxmpaugm.sHtML

[R06] 判断命令是否存在
来源：http://www.share.hesvh.cn/Article/details/gdskowkbb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gxnkpqfwf.sHtML

[R07] if 判断文件
来源：http://3g.zdbjq.cn/Article/details/gnkfqejud.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fehbvm.com/Article/details/gmhnswfkk.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/gphnqiwsa.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fehbvm.com/Article/details/gzvdvwcqc.sHtML

[R09] 字符串比较
来源：http://wap.fehbvm.com/Article/details/gnlfqfypc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.zdbjq.cn/Article/details/ghhaelkhn.sHtML

[R10] 正则匹配
来源：http://mobile.fehbvm.com/Article/details/gefcomruw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.hesvh.cn/Article/details/gvwmbxwgc.sHtML

[R11] case 多分支
来源：http://3g.hesvh.cn/Article/details/gcfznuqdx.sHtML

case "$1" in
来源：http://www.blog.fehbvm.com/Article/details/gfvtvljrg.sHtML

start) echo "启动" ;;
来源：http://read.share.zdbjq.cn/Article/details/gnbaxbtpx.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fehbvm.com/Article/details/gqwkovhaf.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.hesvh.cn/Article/details/gbvqqfkxk.sHtML

esac
来源：http://www.share.fehbvm.com/Article/details/grxfrrrtc.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/gajbbqpkw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.zdbjq.cn/Article/details/gcjmvmwaj.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/glakgcvtf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gynnejyjg.sHtML

[R14] C 风格 for
来源：http://mobile.zdbjq.cn/Article/details/ggjeqtjhd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gcwjsmknr.sHtML

[R15] while 逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/garvnneea.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fehbvm.com/Article/details/gupxjopll.sHtML

[R16] until 等待条件
来源：http://baike.fehbvm.com/Article/details/gqjlogvjm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gdjjzitdh.sHtML

[R17] 数组定义与取值
来源：http://www.share.zdbjq.cn/Article/details/gtexkvkfq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.hesvh.cn/Article/details/givdzbyda.sHtML

[R18] 遍历数组
来源：http://www.share.zdbjq.cn/Article/details/ghijpoexs.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.zdbjq.cn/Article/details/gsrhglyaq.sHtML

[R19] 数组长度
来源：http://3g.fehbvm.com/Article/details/gjwdzprte.sHtML

echo "${#arr[@]}"
来源：http://www.blog.zdbjq.cn/Article/details/gukxqdwab.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fehbvm.com/Article/details/ghrwyxwst.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.zdbjq.cn/Article/details/gfajnntqe.sHtML

[R21] 字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/ghnjrnuwy.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/gltaurumq.sHtML

[R22] 截取子串
来源：http://baike.hesvh.cn/Article/details/ggpvujwkr.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fehbvm.com/Article/details/gjfedgugk.sHtML

[R23] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gigarsmqt.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/gojgzozcm.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gwowicfky.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.hesvh.cn/Article/details/gvajorqyj.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.zdbjq.cn/Article/details/gpeezyztk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fehbvm.com/Article/details/gchsbmplv.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/gjykurvon.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/gtsbezjgo.sHtML

[R27] 算术展开
来源：http://3g.fehbvm.com/Article/details/gziptxyqg.sHtML

echo $((1 + 2 * 3))
来源：http://3g.zdbjq.cn/Article/details/gfsxccedw.sHtML

[R28] 浮点运算
来源：http://read.share.hesvh.cn/Article/details/gskdsvaco.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fehbvm.com/Article/details/gureiioot.sHtML

[R29] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gwtyvcfcr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fehbvm.com/Article/details/gwnrrjfji.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.hesvh.cn/Article/details/guhpwyjeo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.zdbjq.cn/Article/details/gijowvows.sHtML

[R31] 局部变量
来源：http://read.share.zdbjq.cn/Article/details/gbktxllgi.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.hesvh.cn/Article/details/ggxeykaoa.sHtML

[R32] 参数个数校验
来源：http://www.share.fehbvm.com/Article/details/ghuikxbxv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gkccgagls.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/gbikcthsk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.hesvh.cn/Article/details/gckzlyhop.sHtML

[R34] 退出时清理
来源：http://mobile.fehbvm.com/Article/details/gkidvreya.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gwpljxghb.sHtML

[R35] 后台执行并等待
来源：http://baike.zdbjq.cn/Article/details/gvyhfbwmx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fehbvm.com/Article/details/gqujownsf.sHtML

[R36] 并发执行多个任务
来源：http://blog.zdbjq.cn/Article/details/goqewumfq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.zdbjq.cn/Article/details/gtbcismal.sHtML

[R37] 把输出赋给变量
来源：http://www.share.zdbjq.cn/Article/details/gxbypjpcs.sHtML

files=$(ls -1)
来源：http://blog.hesvh.cn/Article/details/ghvwyfshz.sHtML

[R38] 管道串联
来源：http://wap.zdbjq.cn/Article/details/gkfuipzxu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fehbvm.com/Article/details/gzgrrrytk.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fehbvm.com/Article/details/gmovwyigw.sHtML

cmd > out.log 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gerucksyv.sHtML

[R40] 追加写日志
来源：http://3g.fehbvm.com/Article/details/gdafbhdzs.sHtML

echo "log" >> out.log
来源：http://www.blog.zdbjq.cn/Article/details/ghazsuwlr.sHtML

[R41] 丢弃输出
来源：http://mobile.hesvh.cn/Article/details/gbmmwrhwr.sHtML

cmd >/dev/null 2>&1
来源：http://baike.hesvh.cn/Article/details/gevarcwsa.sHtML

[R42] 输入重定向
来源：http://read.share.hesvh.cn/Article/details/gxrpekhry.sHtML

wc -l < a.txt
来源：http://read.share.hesvh.cn/Article/details/gmridjofu.sHtML

[R43] 按名字查找文件
来源：http://blog.fehbvm.com/Article/details/gkmitbzip.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/ghrjthzyl.sHtML

[R44] 按修改时间查找
来源：http://www.share.fehbvm.com/Article/details/grwjtsnjt.sHtML

find . -mtime -7 -type f
来源：http://3g.hesvh.cn/Article/details/gskwkdknh.sHtML

[R45] 批量删除
来源：http://www.share.zdbjq.cn/Article/details/gtfcrtabb.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.zdbjq.cn/Article/details/gmwiyswmk.sHtML

[R46] 递归替换文件内容
来源：http://mobile.zdbjq.cn/Article/details/gtzadjysf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.hesvh.cn/Article/details/gssvqdngo.sHtML

[R47] sed 单行替换
来源：http://blog.hesvh.cn/Article/details/gljaedvcg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gfwmyyyhy.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fehbvm.com/Article/details/gwchgsuky.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gywxskrap.sHtML

[R49] awk 带条件
来源：http://mobile.zdbjq.cn/Article/details/gpbwfzdeu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/gxeucuhgi.sHtML

[R50] awk 求和
来源：http://baike.zdbjq.cn/Article/details/gktgocesc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/goeygazwb.sHtML

[R51] 排序去重取前几
来源：http://mobile.hesvh.cn/Article/details/gatohtnlu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.hesvh.cn/Article/details/gqjwkzxsd.sHtML

[R52] 统计行数
来源：http://baike.hesvh.cn/Article/details/gurnvuuml.sHtML

wc -l a.txt
来源：http://m.share.fehbvm.com/Article/details/gmmkqymxt.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.zdbjq.cn/Article/details/ghtrwgige.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.zdbjq.cn/Article/details/gjyktipmy.sHtML

[R54] 比较两个文件
来源：http://wap.hesvh.cn/Article/details/glduvqslx.sHtML

diff a.txt b.txt
来源：http://wap.zdbjq.cn/Article/details/gwpoxrjui.sHtML

[R55] 压缩与解压
来源：http://www.m.share.hesvh.cn/Article/details/gprsppbny.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.hesvh.cn/Article/details/ggloozwxr.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/gxfhzxnrg.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/gadwwjzlz.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/gvdveqend.sHtML

ssh user@host 'uptime'
来源：http://m.share.hesvh.cn/Article/details/gbdvlmjzk.sHtML

[R58] 下载文件
来源：http://www.m.share.fehbvm.com/Article/details/gqwwcxoku.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fehbvm.com/Article/details/gijjtcuvd.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gpmxbmxbs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.zdbjq.cn/Article/details/gkzowrsai.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/grbmwesed.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fehbvm.com/Article/details/gkfjwputz.sHtML

[R61] 磁盘占用
来源：http://3g.hesvh.cn/Article/details/gbzvkhhmc.sHtML

df -h;  du -sh *
来源：http://www.blog.hesvh.cn/Article/details/gxwjwpzuq.sHtML

[R62] 找最占空间的文件
来源：http://3g.zdbjq.cn/Article/details/gbasvugkh.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.zdbjq.cn/Article/details/grypodztm.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/gfjbmkkjw.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.hesvh.cn/Article/details/gzuhbzibs.sHtML

[R64] 结束进程
来源：http://wap.hesvh.cn/Article/details/gmmpmkwre.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.zdbjq.cn/Article/details/gxmhoyxqo.sHtML

[R65] 查看端口占用
来源：http://3g.zdbjq.cn/Article/details/gkqjuguit.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/ghgjxtjmi.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/glsfjylid.sHtML

crontab -e;  crontab -l
来源：http://m.share.hesvh.cn/Article/details/gtgfohnwd.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/gowsetdto.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/gqypnkzpw.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/gmyzrrtqu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.zdbjq.cn/Article/details/gojhznapj.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/gipaohcnx.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.zdbjq.cn/Article/details/gkpflfbhd.sHtML

[R70] 时间戳与互转
来源：http://mobile.zdbjq.cn/Article/details/gwuvugsit.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/gbmxllvzm.sHtML

[R71] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gppfsxxdo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/grezimsvw.sHtML

[R72] 等待端口就绪
来源：http://read.share.fehbvm.com/Article/details/gjttcyvxe.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gmidficwa.sHtML

[R73] 分割大日志
来源：http://www.blog.fehbvm.com/Article/details/gfopuzqhy.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fehbvm.com/Article/details/gexcyjxlo.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/gnshanepo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gcxzbemut.sHtML

[R75] 导出环境变量
来源：http://wap.zdbjq.cn/Article/details/gissdlhly.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.hesvh.cn/Article/details/grtdkamlp.sHtML

[R76] 使用临时文件
来源：http://wap.fehbvm.com/Article/details/gyyeneaex.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gxkhowrdl.sHtML

[R77] 读取用户输入
来源：http://www.share.fehbvm.com/Article/details/gwwbezpqx.sHtML

read -rp "请输入: " ans
来源：http://mobile.zdbjq.cn/Article/details/gptkrceai.sHtML

[R78] 交互式菜单
来源：http://read.share.hesvh.cn/Article/details/gzptmmsau.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/gaorbrqxp.sHtML

[R79] 解析命令行选项
来源：http://mobile.hesvh.cn/Article/details/ggoywzqhj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.hesvh.cn/Article/details/gpdujknlw.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/gunupurxs.sHtML

time ./run.sh
来源：http://www.share.fehbvm.com/Article/details/gychehkmq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtdsgbvxf.sHtML

S. C / C++ 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gkbywrutz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/giunlaokk.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gmndxkipe.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/gdkphwxsd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fehbvm.com/Article/details/gxzdxivse.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/grqduksor.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.zdbjq.cn/Article/details/gpplartkc.sHtML

[S03] C：读入整数
来源：http://m.share.zdbjq.cn/Article/details/gkvuvnldp.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fehbvm.com/Article/details/gkpooxyai.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/gbcutqyni.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.zdbjq.cn/Article/details/gbpmmbpod.sHtML

[S05] C：字符串长度
来源：http://mobile.hesvh.cn/Article/details/gmhjhafuw.sHtML

strlen(s)
来源：http://read.share.hesvh.cn/Article/details/gacsvizbb.sHtML

[S06] C：字符串比较
来源：http://read.share.zdbjq.cn/Article/details/ggqnghgjb.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/gttawtgdg.sHtML

[S07] C：数组遍历求和
来源：http://baike.zdbjq.cn/Article/details/gthkleizl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fehbvm.com/Article/details/gstemrtrp.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.hesvh.cn/Article/details/grybznllt.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/gscvqpyop.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/glxkkevsg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/gsocmbiym.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/gcpnlkzjx.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.hesvh.cn/Article/details/goenfycjt.sHtML

[S11] C：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gfqvinrfb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.hesvh.cn/Article/details/gwzhgxcde.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fehbvm.com/Article/details/gpoavxrmh.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gioomyitq.sHtML

[S12] C：写文件
来源：http://m.share.zdbjq.cn/Article/details/gutdigsoj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gqcsofsjx.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/gyeoroyyu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fehbvm.com/Article/details/gptzljzml.sHtML

[S14] C：枚举
来源：http://blog.zdbjq.cn/Article/details/grmbllpcd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.zdbjq.cn/Article/details/gswaidhnu.sHtML

[S15] C：类型转换
来源：http://mobile.hesvh.cn/Article/details/gnyvnhmak.sHtML

(double) a / b
来源：http://www.blog.fehbvm.com/Article/details/grdbtqgnh.sHtML

[S16] C：位操作置位
来源：http://baike.fehbvm.com/Article/details/gshpikwaj.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/gvseeyqwc.sHtML

[S17] C：安全拼接字符串
来源：http://wap.hesvh.cn/Article/details/gbnjndnkv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.hesvh.cn/Article/details/gkaewwnmk.sHtML

[S18] C：命令行参数
来源：http://m.share.hesvh.cn/Article/details/gtwcaavjl.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.hesvh.cn/Article/details/gnmwetstq.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/gwlgzxalf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gorqzedpj.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/gyoukuron.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gfuaqifzf.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fehbvm.com/Article/details/giugfzgry.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.zdbjq.cn/Article/details/gtdxhvspf.sHtML

[S22] C：字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/giopghndf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/grsfmvyeb.sHtML

[S23] C：随机数
来源：http://baike.hesvh.cn/Article/details/gvkauvlhm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/gmpiskrah.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/gwjyhlhve.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/gcpchtmwr.sHtML

[S25] C：内存拷贝
来源：http://mobile.zdbjq.cn/Article/details/gyzfbsqjw.sHtML

memcpy(dst, src, n);
来源：http://www.share.fehbvm.com/Article/details/gmnjzbzew.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/gubskftlg.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.hesvh.cn/Article/details/gligghuon.sHtML

[S27] C：定义常量
来源：http://baike.zdbjq.cn/Article/details/gpshuvqku.sHtML

const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gfmpitqti.sHtML

[S28] C：静态变量
来源：http://baike.zdbjq.cn/Article/details/gkahdwqik.sHtML

static int counter = 0;
来源：http://read.share.hesvh.cn/Article/details/gfjsohfwg.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/gmclidacr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.zdbjq.cn/Article/details/gblmyalcs.sHtML

[S30] C：头文件保护
来源：http://read.share.hesvh.cn/Article/details/gqyoglgcq.sHtML

#ifndef X_H
来源：http://blog.zdbjq.cn/Article/details/gbtincimi.sHtML

#define X_H
来源：http://m.share.fehbvm.com/Article/details/gouhjjcpl.sHtML

#endif
来源：http://wap.zdbjq.cn/Article/details/gevlaegur.sHtML

[S31] C++：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gucsqewis.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/gzkjdosok.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fehbvm.com/Article/details/gwvwxnmmw.sHtML

[S32] C++：字符串
来源：http://www.m.share.hesvh.cn/Article/details/gzwafcgxe.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fehbvm.com/Article/details/gkceymetm.sHtML

[S33] C++：vector 增删
来源：http://blog.zdbjq.cn/Article/details/gxuxcylrj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/gnrovkayl.sHtML

[S34] C++：遍历 vector
来源：http://3g.fehbvm.com/Article/details/goyjdzszm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.zdbjq.cn/Article/details/gpjtsfzkl.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/gbsjmtfmc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/ginomeztl.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/gbwbjnoep.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/geuracyyg.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/gqblyiren.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fehbvm.com/Article/details/gkryhjmpc.sHtML

[S38] C++：排序
来源：http://www.blog.fehbvm.com/Article/details/gipxmngcy.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.hesvh.cn/Article/details/gumyaxjsz.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.hesvh.cn/Article/details/gfnfrplwu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.zdbjq.cn/Article/details/gvhdwpblr.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/ghjqzoewi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/gbfkkqkuu.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fehbvm.com/Article/details/gtmevphdo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.hesvh.cn/Article/details/gzshvicyp.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fehbvm.com/Article/details/gcxzzebya.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.zdbjq.cn/Article/details/gnsghepil.sHtML

[S43] C++：智能指针
来源：http://www.share.hesvh.cn/Article/details/gdlceosvr.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fehbvm.com/Article/details/gaeadgklk.sHtML

[S44] C++：引用传参
来源：http://baike.fehbvm.com/Article/details/gwrdnycch.sHtML

void inc(int &x) { ++x; }
来源：http://wap.zdbjq.cn/Article/details/gptdhtckc.sHtML

[S45] C++：lambda
来源：http://baike.zdbjq.cn/Article/details/gvgofdneo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fehbvm.com/Article/details/gethywttb.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/gvmzglfnd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.hesvh.cn/Article/details/gmwbuqzqh.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.hesvh.cn/Article/details/gnsrxlvos.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fehbvm.com/Article/details/gxgidafia.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gpqpfkivk.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.hesvh.cn/Article/details/gddvftdmr.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fehbvm.com/Article/details/gkwohrsgo.sHtML

[S49] C++：写文件
来源：http://www.share.hesvh.cn/Article/details/gmwwbftoe.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.zdbjq.cn/Article/details/gudnwizgb.sHtML

[S50] C++：格式化数字
来源：http://baike.fehbvm.com/Article/details/gaxxrhiga.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/ghveogxbj.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/gqsoneoph.sHtML

static_cast<double>(a) / b
来源：http://wap.fehbvm.com/Article/details/gabkbegvo.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.zdbjq.cn/Article/details/gnvwclwiu.sHtML


<!-- 参考信息 -->