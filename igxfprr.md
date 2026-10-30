代发 wailian999

[Q82] 字符长度与字节长度
来源：http://read.share.fehbvm.com/Article/details/gjxcodhoc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gjffilbwg.sHtML

[Q83] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gfrhxzdnm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gqicofytv.sHtML

[Q84] 去除首尾空格
来源：http://wap.hesvh.cn/Article/details/gldinyjds.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/grmwaqdie.sHtML

[Q85] 数值取整
来源：http://blog.hesvh.cn/Article/details/goqhfkhen.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fehbvm.com/Article/details/ggcllmths.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/gfqpahmgp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fehbvm.com/Article/details/gtjsndljt.sHtML

[Q87] JSON 字段做条件
来源：http://wap.zdbjq.cn/Article/details/ggunlwhzi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.hesvh.cn/Article/details/gceylfoaf.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.hesvh.cn/Article/details/gejqmeaoq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fehbvm.com/Article/details/gfgsxbqsf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fehbvm.com/Article/details/goaonakgn.sHtML

[Q89] 判断表是否存在
来源：http://m.share.hesvh.cn/Article/details/guyfguofp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.hesvh.cn/Article/details/gdzqpkbsd.sHtML

[Q90] 生成序号列
来源：http://blog.fehbvm.com/Article/details/gnwcunojw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.hesvh.cn/Article/details/gifjlinjm.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/guzmsinqp.sHtML

R. Bash 专题
来源：http://m.share.hesvh.cn/Article/details/gqpenleiw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gftgxwgfe.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fehbvm.com/Article/details/gksdzrwiq.sHtML

#!/usr/bin/env bash
来源：http://mobile.fehbvm.com/Article/details/ghqnfwqjf.sHtML

set -euo pipefail
来源：http://mobile.hesvh.cn/Article/details/gmnclcali.sHtML

[R02] 变量赋值与使用
来源：http://blog.zdbjq.cn/Article/details/gtxvrdjlf.sHtML

name="Tom"; echo "$name"
来源：http://baike.hesvh.cn/Article/details/gxkurrmwf.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/ghccihmje.sHtML

readonly PI=3.14
来源：http://www.blog.hesvh.cn/Article/details/grjbfvmiy.sHtML

[R04] 位置参数
来源：http://read.share.zdbjq.cn/Article/details/gxhueyqcg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.zdbjq.cn/Article/details/gvsccwoqp.sHtML

[R05] 参数默认值
来源：http://blog.hesvh.cn/Article/details/gommbiwad.sHtML

name="${1:-default}"
来源：http://mobile.hesvh.cn/Article/details/gxivdcnnp.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gwnzwvkjy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gtnvlqrfn.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/gyrgqinor.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/gulhgxnco.sHtML

[R08] 数值比较
来源：http://blog.zdbjq.cn/Article/details/ghwnjbqjg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gjznngjkx.sHtML

[R09] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/gkxouhndd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gqvqbhmri.sHtML

[R10] 正则匹配
来源：http://www.m.share.fehbvm.com/Article/details/gsuohuywz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gyvxvwges.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/gkywkjrpj.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/gfipbwfio.sHtML

start) echo "启动" ;;
来源：http://3g.hesvh.cn/Article/details/gwlsqvajj.sHtML

stop)  echo "停止" ;;
来源：http://3g.hesvh.cn/Article/details/gqzmciuoz.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fehbvm.com/Article/details/gnjqboyol.sHtML

esac
来源：http://baike.zdbjq.cn/Article/details/gpyoqvxcv.sHtML

[R12] for 遍历文件
来源：http://baike.zdbjq.cn/Article/details/gxpqjikuy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fehbvm.com/Article/details/gugvtwqfk.sHtML

[R13] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/gctxqmyau.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gcfpcroql.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/gyekneitz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gskbfhxqd.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gocblpyic.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.hesvh.cn/Article/details/gxkvpskts.sHtML

[R16] until 等待条件
来源：http://www.m.share.hesvh.cn/Article/details/gnsnxbjsd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gqgydomki.sHtML

[R17] 数组定义与取值
来源：http://www.blog.zdbjq.cn/Article/details/gqskfvlya.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fehbvm.com/Article/details/gzoknupaa.sHtML

[R18] 遍历数组
来源：http://wap.fehbvm.com/Article/details/gpdltdhsu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fehbvm.com/Article/details/ghoyioizq.sHtML

[R19] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gaqnxaoui.sHtML

echo "${#arr[@]}"
来源：http://mobile.hesvh.cn/Article/details/gmrhmattq.sHtML

[R20] 关联数组（字典）
来源：http://wap.hesvh.cn/Article/details/glgsvyknq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fehbvm.com/Article/details/gdsgcwanq.sHtML

[R21] 字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gstbguvtx.sHtML

echo "${#s}"
来源：http://read.share.fehbvm.com/Article/details/gszbxjvxb.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gkwwzlcuk.sHtML

echo "${s:0:5}"
来源：http://read.share.hesvh.cn/Article/details/gadxlphch.sHtML

[R23] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/geeyazcfy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.hesvh.cn/Article/details/gfyqcvcmp.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gyezzxzlx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.zdbjq.cn/Article/details/gqnkjclal.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fehbvm.com/Article/details/gnxxihfgc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.hesvh.cn/Article/details/gixgkqfub.sHtML

[R26] 命令替换
来源：http://wap.zdbjq.cn/Article/details/gbvshoygq.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/gdfykbrga.sHtML

[R27] 算术展开
来源：http://www.share.hesvh.cn/Article/details/gifwfnuwc.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.zdbjq.cn/Article/details/ggcnnqquo.sHtML

[R28] 浮点运算
来源：http://mobile.hesvh.cn/Article/details/gzknoporc.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.zdbjq.cn/Article/details/geidvvase.sHtML

[R29] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gluwtgzii.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/gvqcwboop.sHtML

[R30] 函数返回状态码
来源：http://baike.fehbvm.com/Article/details/gnpfxmwwt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.zdbjq.cn/Article/details/gtpotrisa.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/gmblgtgcr.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.hesvh.cn/Article/details/giphgtyyi.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/gpzxjtcen.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gnefszybp.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/ghulxudal.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fehbvm.com/Article/details/ggyysulkl.sHtML

[R34] 退出时清理
来源：http://read.share.fehbvm.com/Article/details/gbotnwnsz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gbqmlbpsk.sHtML

[R35] 后台执行并等待
来源：http://blog.fehbvm.com/Article/details/grykbybho.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.hesvh.cn/Article/details/gvezsglse.sHtML

[R36] 并发执行多个任务
来源：http://3g.zdbjq.cn/Article/details/gsxjtofyq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fehbvm.com/Article/details/glfxskude.sHtML

[R37] 把输出赋给变量
来源：http://www.share.zdbjq.cn/Article/details/gghgpspxp.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/gebfozdjo.sHtML

[R38] 管道串联
来源：http://www.blog.zdbjq.cn/Article/details/gcifvawei.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.zdbjq.cn/Article/details/gufiumxsf.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/ggtluiswp.sHtML

cmd > out.log 2>&1
来源：http://mobile.fehbvm.com/Article/details/gzgexilby.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/gagvujehi.sHtML

echo "log" >> out.log
来源：http://3g.hesvh.cn/Article/details/gpjukqkdj.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fehbvm.com/Article/details/gaxpbrunn.sHtML

cmd >/dev/null 2>&1
来源：http://baike.hesvh.cn/Article/details/gdrzydkhy.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/gvspbdecj.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/gsmigetxg.sHtML

[R43] 按名字查找文件
来源：http://m.share.hesvh.cn/Article/details/gyjvhhlnz.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/gevlijwct.sHtML

[R44] 按修改时间查找
来源：http://wap.zdbjq.cn/Article/details/gzlofkjgo.sHtML

find . -mtime -7 -type f
来源：http://read.share.hesvh.cn/Article/details/gktwvygtk.sHtML

[R45] 批量删除
来源：http://www.blog.zdbjq.cn/Article/details/gaaatdeve.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/gbgskacit.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fehbvm.com/Article/details/glviicyrk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fehbvm.com/Article/details/guoueavrg.sHtML

[R47] sed 单行替换
来源：http://www.blog.hesvh.cn/Article/details/gwfxprzqn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.hesvh.cn/Article/details/gwkeuhgse.sHtML

[R48] awk 取指定列
来源：http://blog.zdbjq.cn/Article/details/gandhmwqo.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fehbvm.com/Article/details/grwrfushw.sHtML

[R49] awk 带条件
来源：http://blog.fehbvm.com/Article/details/gkdizdvti.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.hesvh.cn/Article/details/gkiasvpxx.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/guagpgent.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gfrsmacat.sHtML

[R51] 排序去重取前几
来源：http://www.share.hesvh.cn/Article/details/gmoczubgc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.zdbjq.cn/Article/details/gguevvton.sHtML

[R52] 统计行数
来源：http://mobile.fehbvm.com/Article/details/gzjoznkmj.sHtML

wc -l a.txt
来源：http://3g.zdbjq.cn/Article/details/gokkjjsso.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fehbvm.com/Article/details/gxlmacmat.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/gkrqxyntr.sHtML

[R54] 比较两个文件
来源：http://mobile.fehbvm.com/Article/details/gzdvzonns.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/gilpztfva.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fehbvm.com/Article/details/gecjfyddx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.hesvh.cn/Article/details/gxgauzqkb.sHtML

[R56] 远程拷贝
来源：http://www.blog.fehbvm.com/Article/details/gpatnbupj.sHtML

scp file user@host:/path/
来源：http://www.share.fehbvm.com/Article/details/gvfaaarkl.sHtML

[R57] 远程执行命令
来源：http://mobile.zdbjq.cn/Article/details/gvqbfobvw.sHtML

ssh user@host 'uptime'
来源：http://blog.zdbjq.cn/Article/details/ggsehlorg.sHtML

[R58] 下载文件
来源：http://wap.zdbjq.cn/Article/details/gkpbtogvb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fehbvm.com/Article/details/gfvzjzjzu.sHtML

[R59] 发 POST JSON
来源：http://m.share.hesvh.cn/Article/details/glnmezpjo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.hesvh.cn/Article/details/gxindclhh.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gjizwjgpg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fehbvm.com/Article/details/giodapxzn.sHtML

[R61] 磁盘占用
来源：http://3g.fehbvm.com/Article/details/gwnibvkdw.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/gzozdsixt.sHtML

[R62] 找最占空间的文件
来源：http://blog.hesvh.cn/Article/details/gihfwwbwz.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fehbvm.com/Article/details/gqznadpye.sHtML

[R63] 内存与进程
来源：http://www.blog.zdbjq.cn/Article/details/gizfapboc.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.hesvh.cn/Article/details/gisvunwlp.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/gitxlbwrf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fehbvm.com/Article/details/gkxtzdsbm.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/gmgvlxhiz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.zdbjq.cn/Article/details/glbmhvcdn.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gbkxxtkkc.sHtML

crontab -e;  crontab -l
来源：http://www.blog.zdbjq.cn/Article/details/gqbpdlmfe.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fehbvm.com/Article/details/gbjnutjrt.sHtML

openssl rand -hex 16
来源：http://mobile.fehbvm.com/Article/details/gdvdrzqxh.sHtML

[R68] 计算文件校验值
来源：http://baike.hesvh.cn/Article/details/gykuzehxu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.zdbjq.cn/Article/details/gwrseuqrs.sHtML

[R69] 生成随机密码
来源：http://mobile.fehbvm.com/Article/details/gfhwrcufq.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/gxqmpcyxr.sHtML

[R70] 时间戳与互转
来源：http://baike.hesvh.cn/Article/details/gvubhqmmx.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.zdbjq.cn/Article/details/gpddcaypp.sHtML

[R71] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gdczxooim.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/gvfnhvczp.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fehbvm.com/Article/details/grsptqnzi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gwvcelalq.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/gecxwclcs.sHtML

split -l 1000 big.log part_
来源：http://3g.fehbvm.com/Article/details/gpxegkcqd.sHtML

[R74] 批量重命名
来源：http://blog.fehbvm.com/Article/details/gfacpctyk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fehbvm.com/Article/details/gcaqorikk.sHtML

[R75] 导出环境变量
来源：http://wap.zdbjq.cn/Article/details/grjytqjyl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/gjcufkrkp.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fehbvm.com/Article/details/gqpqkheiv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gnicrwxcx.sHtML

[R77] 读取用户输入
来源：http://mobile.zdbjq.cn/Article/details/gtyjzvzlo.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/getgzmozz.sHtML

[R78] 交互式菜单
来源：http://read.share.zdbjq.cn/Article/details/gxzjmmgmz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/gohehzhdm.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fehbvm.com/Article/details/gsykhiucy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.zdbjq.cn/Article/details/gpjuopiek.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/gytoxkcaq.sHtML

time ./run.sh
来源：http://www.share.hesvh.cn/Article/details/gzgznzazg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gatwxohft.sHtML

S. C / C++ 专题
来源：http://m.share.fehbvm.com/Article/details/gktrvksrt.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gdmrxydjs.sHtML

[S01] C：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gjdoepyck.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/gjvsiqpws.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/gwrtjdkla.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.hesvh.cn/Article/details/gxkmmskkk.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fehbvm.com/Article/details/gzvjzhhga.sHtML

[S03] C：读入整数
来源：http://read.share.fehbvm.com/Article/details/grnfcjxri.sHtML

int x; scanf("%d", &x);
来源：http://wap.zdbjq.cn/Article/details/galstakvz.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/gwpcpbvvg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fehbvm.com/Article/details/gproefxij.sHtML

[S05] C：字符串长度
来源：http://3g.hesvh.cn/Article/details/gqxeqruub.sHtML

strlen(s)
来源：http://www.blog.hesvh.cn/Article/details/gkjehqsdj.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/gnodrwixu.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/gddavzkyt.sHtML

[S07] C：数组遍历求和
来源：http://3g.fehbvm.com/Article/details/gpzdraazj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.zdbjq.cn/Article/details/gepuknhni.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/glyhyebva.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.hesvh.cn/Article/details/gnomqdqfn.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fehbvm.com/Article/details/gpuvxqmdt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/gtkijhish.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.zdbjq.cn/Article/details/gghydmnxi.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.hesvh.cn/Article/details/gfketueqn.sHtML

[S11] C：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gjhofvfcj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.hesvh.cn/Article/details/gycloshfj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gvflwppmf.sHtML

fclose(f);
来源：http://baike.zdbjq.cn/Article/details/ghhdgiswx.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gwhodpjtb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gbuvngoad.sHtML

[S13] C：宏定义
来源：http://wap.fehbvm.com/Article/details/gupjckkru.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/ghjdzlwtw.sHtML

[S14] C：枚举
来源：http://wap.hesvh.cn/Article/details/glattloxy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.hesvh.cn/Article/details/gupcghtnp.sHtML

[S15] C：类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gefxxufhx.sHtML

(double) a / b
来源：http://baike.hesvh.cn/Article/details/gpsqmiubq.sHtML

[S16] C：位操作置位
来源：http://baike.fehbvm.com/Article/details/gldhwuxxh.sHtML

x |= (1 << 3);
来源：http://www.share.hesvh.cn/Article/details/gulpdfebi.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gwhmivqew.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fehbvm.com/Article/details/gwqtgheob.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gdwurqonm.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/gkvtuabrc.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/gftowkrru.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gquzqkpia.sHtML

[S20] C：二分查找
来源：http://mobile.zdbjq.cn/Article/details/gcsbgdyif.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gztifailk.sHtML

[S21] C：字符类别判断
来源：http://www.share.hesvh.cn/Article/details/gvrgtzknu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fehbvm.com/Article/details/gwiyyywhc.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/guoozwosa.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/gcvrmjffb.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/gwhtqdpur.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.zdbjq.cn/Article/details/gvzrhrbzd.sHtML

[S24] C：获取本地时间
来源：http://baike.zdbjq.cn/Article/details/ggkykywxa.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.hesvh.cn/Article/details/gncudeurv.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/gvpvauwuc.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fehbvm.com/Article/details/gfnuagsdl.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/gthvrutwp.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fehbvm.com/Article/details/gskihwjwu.sHtML

[S27] C：定义常量
来源：http://www.blog.zdbjq.cn/Article/details/ggdvjcrgb.sHtML

const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gbnagqkfn.sHtML

[S28] C：静态变量
来源：http://www.share.fehbvm.com/Article/details/gbigvkpan.sHtML

static int counter = 0;
来源：http://blog.fehbvm.com/Article/details/gpmbhcgwm.sHtML

[S29] C：变参函数
来源：http://www.m.share.zdbjq.cn/Article/details/gofibhsau.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.hesvh.cn/Article/details/gebdfcion.sHtML

[S30] C：头文件保护
来源：http://www.share.fehbvm.com/Article/details/gpjixskrb.sHtML

#ifndef X_H
来源：http://blog.hesvh.cn/Article/details/glngfcbjk.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/gpordogoc.sHtML

#endif
来源：http://blog.hesvh.cn/Article/details/gnmnxxfja.sHtML

[S31] C++：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gzzdndeuv.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/gokcjzngq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/gnoznzawq.sHtML

[S32] C++：字符串
来源：http://www.blog.zdbjq.cn/Article/details/gbyyvydwh.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.hesvh.cn/Article/details/gbbghunxq.sHtML

[S33] C++：vector 增删
来源：http://blog.fehbvm.com/Article/details/gnlgsikjx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/godxfvixc.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/grexpmyso.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.zdbjq.cn/Article/details/gizhccmjd.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/geystbjbt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gvutfxuhl.sHtML

[S36] C++：unordered_map
来源：http://baike.fehbvm.com/Article/details/glxyyjwec.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gjhmjkhwd.sHtML

[S37] C++：set
来源：http://blog.hesvh.cn/Article/details/gxovdxoup.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fehbvm.com/Article/details/gzpbbrmol.sHtML

[S38] C++：排序
来源：http://www.m.share.zdbjq.cn/Article/details/gevuetoex.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gpgwbwsxi.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.zdbjq.cn/Article/details/googfcwiz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/gponoshlu.sHtML

[S40] C++：查找元素
来源：http://mobile.fehbvm.com/Article/details/gksbvxcvt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/gegbaakfe.sHtML

[S41] C++：类与构造函数
来源：http://3g.fehbvm.com/Article/details/gxggepsun.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.hesvh.cn/Article/details/gszxqqkss.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.zdbjq.cn/Article/details/gwpdwvuli.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.zdbjq.cn/Article/details/gyancheiw.sHtML

[S43] C++：智能指针
来源：http://wap.hesvh.cn/Article/details/gberqouww.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fehbvm.com/Article/details/geokssgoa.sHtML

[S44] C++：引用传参
来源：http://www.blog.fehbvm.com/Article/details/ghzprqpgi.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gophjpszy.sHtML

[S45] C++：lambda
来源：http://m.share.fehbvm.com/Article/details/gkxqhqpyq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/gcyonhcei.sHtML

[S46] C++：函数模板
来源：http://m.share.hesvh.cn/Article/details/gvtwxrqoo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.hesvh.cn/Article/details/gkyggiqgh.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fehbvm.com/Article/details/gaenzuccx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gdjdsrdau.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/grxmfxhhw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/gyltvzins.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/gwgjjlbyc.sHtML

[S49] C++：写文件
来源：http://mobile.hesvh.cn/Article/details/gahzrsxdw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fehbvm.com/Article/details/gsnlxgkue.sHtML

[S50] C++：格式化数字
来源：http://www.share.zdbjq.cn/Article/details/gruotjcfj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gqwpxrisi.sHtML

[S51] C++：显式类型转换
来源：http://mobile.hesvh.cn/Article/details/goiuxdpfr.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gymxqohol.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fehbvm.com/Article/details/gpjeankcw.sHtML


<!-- 参考信息 -->