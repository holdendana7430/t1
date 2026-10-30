代发 wailian999

[Q82] 字符长度与字节长度
来源：http://www.m.share.zdbjq.cn/Article/details/gkfodgynw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/grxiwgred.sHtML

[Q83] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/garnpngkj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gdpcpstgl.sHtML

[Q84] 去除首尾空格
来源：http://wap.hesvh.cn/Article/details/gykzknjzi.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/grjljxvzx.sHtML

[Q85] 数值取整
来源：http://www.share.fehbvm.com/Article/details/gqvwlzpup.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.hesvh.cn/Article/details/gmrxnpuhx.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.zdbjq.cn/Article/details/gqwtwtkpn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.zdbjq.cn/Article/details/gxjrjaldh.sHtML

[Q87] JSON 字段做条件
来源：http://3g.zdbjq.cn/Article/details/gbwrccbfk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.zdbjq.cn/Article/details/gtyakrmwg.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.hesvh.cn/Article/details/giqkuoiqj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fehbvm.com/Article/details/guxuvzrxf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/grvzkulro.sHtML

[Q89] 判断表是否存在
来源：http://www.share.hesvh.cn/Article/details/gsehqxrvy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.zdbjq.cn/Article/details/gwaslrmsf.sHtML

[Q90] 生成序号列
来源：http://m.share.hesvh.cn/Article/details/getmnkzmv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.zdbjq.cn/Article/details/gmyrrejna.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gfstvvyws.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/gbhhilntz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gylqqrkkv.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fehbvm.com/Article/details/goplvmfmb.sHtML

#!/usr/bin/env bash
来源：http://3g.zdbjq.cn/Article/details/gnwtwlbxh.sHtML

set -euo pipefail
来源：http://wap.fehbvm.com/Article/details/gaznfuthl.sHtML

[R02] 变量赋值与使用
来源：http://wap.hesvh.cn/Article/details/gzzrjvnup.sHtML

name="Tom"; echo "$name"
来源：http://wap.zdbjq.cn/Article/details/gjtbqiyka.sHtML

[R03] 只读变量
来源：http://www.m.share.hesvh.cn/Article/details/gqkawparg.sHtML

readonly PI=3.14
来源：http://mobile.zdbjq.cn/Article/details/gikscqsrp.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/grvvqofog.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fehbvm.com/Article/details/gvkqmepdk.sHtML

[R05] 参数默认值
来源：http://wap.zdbjq.cn/Article/details/gnktxdknt.sHtML

name="${1:-default}"
来源：http://wap.zdbjq.cn/Article/details/gidcynmav.sHtML

[R06] 判断命令是否存在
来源：http://baike.hesvh.cn/Article/details/gfzorodwg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gxfxvaccf.sHtML

[R07] if 判断文件
来源：http://3g.hesvh.cn/Article/details/gbmsahzhv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.zdbjq.cn/Article/details/gltwhiscl.sHtML

[R08] 数值比较
来源：http://www.share.fehbvm.com/Article/details/gixatzeam.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.hesvh.cn/Article/details/gygnvcgeu.sHtML

[R09] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/gwvatdoom.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.zdbjq.cn/Article/details/gmmmgfypg.sHtML

[R10] 正则匹配
来源：http://www.m.share.fehbvm.com/Article/details/guvhhvnnz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fehbvm.com/Article/details/ginqysrnl.sHtML

[R11] case 多分支
来源：http://wap.fehbvm.com/Article/details/gxwzhlkud.sHtML

case "$1" in
来源：http://www.m.share.hesvh.cn/Article/details/gvtuqfvcl.sHtML

start) echo "启动" ;;
来源：http://wap.zdbjq.cn/Article/details/gvckqpyde.sHtML

stop)  echo "停止" ;;
来源：http://baike.zdbjq.cn/Article/details/giojqatia.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fehbvm.com/Article/details/gvrdrqbxs.sHtML

esac
来源：http://wap.fehbvm.com/Article/details/glalwmpjh.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/gobqixycn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.hesvh.cn/Article/details/gntkpvuzv.sHtML

[R13] for 计数循环
来源：http://read.share.zdbjq.cn/Article/details/gcldbcqjr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/guquaefvh.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/gzrvarzrx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/geudydmps.sHtML

[R15] while 逐行读文件
来源：http://wap.fehbvm.com/Article/details/gwnqyuifw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.zdbjq.cn/Article/details/gtjikczam.sHtML

[R16] until 等待条件
来源：http://read.share.fehbvm.com/Article/details/gzggngqfp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gyccjivna.sHtML

[R17] 数组定义与取值
来源：http://blog.zdbjq.cn/Article/details/gbxhbdszu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/gtkytwogl.sHtML

[R18] 遍历数组
来源：http://3g.zdbjq.cn/Article/details/gudjjwujf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.zdbjq.cn/Article/details/ghvrjetdm.sHtML

[R19] 数组长度
来源：http://blog.hesvh.cn/Article/details/gnifyqbxh.sHtML

echo "${#arr[@]}"
来源：http://wap.hesvh.cn/Article/details/ggaannpwo.sHtML

[R20] 关联数组（字典）
来源：http://m.share.hesvh.cn/Article/details/gkdbyrhbk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.hesvh.cn/Article/details/groddbhjv.sHtML

[R21] 字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gxlrexgft.sHtML

echo "${#s}"
来源：http://m.share.zdbjq.cn/Article/details/gposccong.sHtML

[R22] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gapwqioml.sHtML

echo "${s:0:5}"
来源：http://wap.zdbjq.cn/Article/details/gplncszsk.sHtML

[R23] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gztqgmarx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/guixrcfnx.sHtML

[R24] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gxscubkot.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.zdbjq.cn/Article/details/gnvdddwbc.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fehbvm.com/Article/details/gpyhaaezt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.zdbjq.cn/Article/details/gbdixwruk.sHtML

[R26] 命令替换
来源：http://wap.zdbjq.cn/Article/details/geatcluej.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/gbhnkdwup.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/goeqewvbx.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fehbvm.com/Article/details/gwkzncosk.sHtML

[R28] 浮点运算
来源：http://www.blog.fehbvm.com/Article/details/guouhkvoc.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fehbvm.com/Article/details/gdqusjypb.sHtML

[R29] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gealhxmcc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fehbvm.com/Article/details/gledqvutw.sHtML

[R30] 函数返回状态码
来源：http://3g.fehbvm.com/Article/details/geuqdnlaw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.hesvh.cn/Article/details/gkunduupv.sHtML

[R31] 局部变量
来源：http://m.share.hesvh.cn/Article/details/gtqfjwfje.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/gwfqpqvbh.sHtML

[R32] 参数个数校验
来源：http://wap.hesvh.cn/Article/details/gxfvnvuzd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gpfwzfsxj.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.zdbjq.cn/Article/details/gumzsqttx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.hesvh.cn/Article/details/gveqizqnj.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/goupuyvqf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/geurklmvh.sHtML

[R35] 后台执行并等待
来源：http://blog.fehbvm.com/Article/details/gtvyukrac.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fehbvm.com/Article/details/gqjxgfsvh.sHtML

[R36] 并发执行多个任务
来源：http://baike.fehbvm.com/Article/details/gxwtnfmvi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fehbvm.com/Article/details/gbeoqaafv.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.hesvh.cn/Article/details/guxdbrgqu.sHtML

files=$(ls -1)
来源：http://blog.hesvh.cn/Article/details/gebuxuhjp.sHtML

[R38] 管道串联
来源：http://read.share.zdbjq.cn/Article/details/gimtlttbe.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/gqlkxjscb.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.zdbjq.cn/Article/details/geliqxonu.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gcazynigo.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/gpoedxqgu.sHtML

echo "log" >> out.log
来源：http://mobile.zdbjq.cn/Article/details/gidjxbzgr.sHtML

[R41] 丢弃输出
来源：http://mobile.fehbvm.com/Article/details/gngcccmgg.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fehbvm.com/Article/details/gtxjaksjd.sHtML

[R42] 输入重定向
来源：http://www.share.fehbvm.com/Article/details/gdlmujnmt.sHtML

wc -l < a.txt
来源：http://mobile.hesvh.cn/Article/details/gohnrdgtx.sHtML

[R43] 按名字查找文件
来源：http://mobile.hesvh.cn/Article/details/gfeejoljt.sHtML

find . -name "*.log" -type f
来源：http://3g.fehbvm.com/Article/details/gnyypqufu.sHtML

[R44] 按修改时间查找
来源：http://read.share.fehbvm.com/Article/details/goybjlvbt.sHtML

find . -mtime -7 -type f
来源：http://blog.fehbvm.com/Article/details/gvdfymujx.sHtML

[R45] 批量删除
来源：http://mobile.hesvh.cn/Article/details/gggvhuzal.sHtML

find . -name "*.tmp" -delete
来源：http://baike.zdbjq.cn/Article/details/guockbppc.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/gfhtdyjbi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fehbvm.com/Article/details/gpuzpexxy.sHtML

[R47] sed 单行替换
来源：http://www.m.share.zdbjq.cn/Article/details/glqckauwf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gqmfwtmfb.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/gzgphmtpd.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gbndmehyu.sHtML

[R49] awk 带条件
来源：http://m.share.fehbvm.com/Article/details/gbbshzbid.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/geccgtyob.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/gvqfphftb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gwvjvjvsj.sHtML

[R51] 排序去重取前几
来源：http://wap.zdbjq.cn/Article/details/getgukgmh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fehbvm.com/Article/details/gvqwgkyhv.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/gzajowdci.sHtML

wc -l a.txt
来源：http://www.share.fehbvm.com/Article/details/gsinfjfwx.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fehbvm.com/Article/details/gspwdjtbe.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.zdbjq.cn/Article/details/gahxhahzb.sHtML

[R54] 比较两个文件
来源：http://read.share.fehbvm.com/Article/details/gzbseglpq.sHtML

diff a.txt b.txt
来源：http://wap.hesvh.cn/Article/details/gayfcopgh.sHtML

[R55] 压缩与解压
来源：http://www.share.hesvh.cn/Article/details/gbxbkrqbs.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fehbvm.com/Article/details/grqktrgqt.sHtML

[R56] 远程拷贝
来源：http://baike.fehbvm.com/Article/details/geqkcjrxb.sHtML

scp file user@host:/path/
来源：http://wap.fehbvm.com/Article/details/gvlifyqmd.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/gttampfeu.sHtML

ssh user@host 'uptime'
来源：http://m.share.hesvh.cn/Article/details/gpeacljpi.sHtML

[R58] 下载文件
来源：http://wap.hesvh.cn/Article/details/govyccsej.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.hesvh.cn/Article/details/glqeekxzm.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/gpwssvshu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.hesvh.cn/Article/details/gilfigtrj.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gjorzxczi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/gnxrqxjuy.sHtML

[R61] 磁盘占用
来源：http://blog.zdbjq.cn/Article/details/gqjjmxiyv.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/gxxkmzbhr.sHtML

[R62] 找最占空间的文件
来源：http://baike.fehbvm.com/Article/details/gkutcjaxf.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fehbvm.com/Article/details/gtqpxjqqo.sHtML

[R63] 内存与进程
来源：http://www.share.zdbjq.cn/Article/details/gbvdajmnd.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/gcmosxiov.sHtML

[R64] 结束进程
来源：http://www.share.zdbjq.cn/Article/details/gnyfnhbuw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.zdbjq.cn/Article/details/gvrznkuxy.sHtML

[R65] 查看端口占用
来源：http://www.m.share.hesvh.cn/Article/details/gcsxxuohq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fehbvm.com/Article/details/gmitdgggl.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/gmqpcsvit.sHtML

crontab -e;  crontab -l
来源：http://blog.zdbjq.cn/Article/details/glxtzcmac.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/gfwhtuffn.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/gtcaxupsk.sHtML

[R68] 计算文件校验值
来源：http://blog.hesvh.cn/Article/details/gpylpheal.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.zdbjq.cn/Article/details/gajxfedqa.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/gygskodai.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.zdbjq.cn/Article/details/gdorwxxrw.sHtML

[R70] 时间戳与互转
来源：http://baike.fehbvm.com/Article/details/gysxyqiym.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.zdbjq.cn/Article/details/gfvcdgcxy.sHtML

[R71] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gceebifem.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fehbvm.com/Article/details/gvevqgsbt.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fehbvm.com/Article/details/gfwcbvexd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gwajczetg.sHtML

[R73] 分割大日志
来源：http://blog.hesvh.cn/Article/details/gfbosznlh.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/gzsedxvop.sHtML

[R74] 批量重命名
来源：http://www.blog.fehbvm.com/Article/details/gcllmkqrk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.hesvh.cn/Article/details/gfdilzvhd.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/grlracsra.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fehbvm.com/Article/details/ghntjvkae.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/gtukfniqm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/giruwajls.sHtML

[R77] 读取用户输入
来源：http://m.share.fehbvm.com/Article/details/gbtbyeuge.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/gtboqokde.sHtML

[R78] 交互式菜单
来源：http://m.share.hesvh.cn/Article/details/gkszdjsjb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/gqqfkbdbb.sHtML

[R79] 解析命令行选项
来源：http://baike.zdbjq.cn/Article/details/gncmnbjvs.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.hesvh.cn/Article/details/gsrpdavia.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.hesvh.cn/Article/details/gqevnsqor.sHtML

time ./run.sh
来源：http://www.m.share.fehbvm.com/Article/details/gugfikmdp.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvfquqqbs.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/gdwmjokhu.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gniavwhum.sHtML

[S01] C：Hello World
来源：http://read.share.zdbjq.cn/Article/details/glavkjjtk.sHtML

#include <stdio.h>
来源：http://read.share.zdbjq.cn/Article/details/glyeapmcb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.hesvh.cn/Article/details/gaekuzalj.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/gueelfavf.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/guhcgmnre.sHtML

[S03] C：读入整数
来源：http://m.share.zdbjq.cn/Article/details/gawcixzph.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/gbnleujyr.sHtML

[S04] C：字符串复制
来源：http://www.m.share.hesvh.cn/Article/details/gmaoaebwo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fehbvm.com/Article/details/gycejzuod.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/gijjxxcql.sHtML

strlen(s)
来源：http://blog.hesvh.cn/Article/details/gvuxvacpe.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/gzfjbqbkf.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/gkumituny.sHtML

[S07] C：数组遍历求和
来源：http://wap.zdbjq.cn/Article/details/gpimcmlqt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.zdbjq.cn/Article/details/gnndbkcsv.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/gdubcukml.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.hesvh.cn/Article/details/gyfmxpspm.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.hesvh.cn/Article/details/gvnljlnql.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.zdbjq.cn/Article/details/gkonfunyn.sHtML

[S10] C：指针与解引用
来源：http://blog.zdbjq.cn/Article/details/gaoixzttw.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gdopflqxs.sHtML

[S11] C：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gikbpcntq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.zdbjq.cn/Article/details/gwvjmkplf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/ggzeemide.sHtML

fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gjfrmltev.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/gcpuaqtqu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gxiznlqul.sHtML

[S13] C：宏定义
来源：http://www.blog.zdbjq.cn/Article/details/gysnjhxip.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/gbqxfxoci.sHtML

[S14] C：枚举
来源：http://m.share.fehbvm.com/Article/details/ghkxbjeid.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.hesvh.cn/Article/details/ghljvqobd.sHtML

[S15] C：类型转换
来源：http://www.blog.hesvh.cn/Article/details/grfbciceb.sHtML

(double) a / b
来源：http://mobile.zdbjq.cn/Article/details/ginwyfjig.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fehbvm.com/Article/details/gcptijeit.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/gsvojeplf.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gpqkvqmcl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.zdbjq.cn/Article/details/gnrnjosue.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/gilomdyaz.sHtML

int main(int argc, char **argv)
来源：http://baike.fehbvm.com/Article/details/grqdwijph.sHtML

[S19] C：快速排序
来源：http://www.blog.fehbvm.com/Article/details/gkimdhfzq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gjsmtzvoq.sHtML

[S20] C：二分查找
来源：http://www.m.share.fehbvm.com/Article/details/giloehpdu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gbjluhgng.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/ggobxtttt.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.zdbjq.cn/Article/details/gwkdrpxks.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gajbvcqrw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.zdbjq.cn/Article/details/gdppnecek.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gnuvncgri.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.hesvh.cn/Article/details/gvzdhtujp.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/gdkfocwle.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.zdbjq.cn/Article/details/grzdeiepx.sHtML

[S25] C：内存拷贝
来源：http://wap.zdbjq.cn/Article/details/ggopgyney.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/geyylpvvn.sHtML

[S26] C：内存清零
来源：http://baike.zdbjq.cn/Article/details/gawdqubdj.sHtML

memset(a, 0, sizeof a);
来源：http://3g.hesvh.cn/Article/details/gbjvqafbe.sHtML

[S27] C：定义常量
来源：http://mobile.hesvh.cn/Article/details/gcxynlizv.sHtML

const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gbbmuxhny.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/gqoplfbzk.sHtML

static int counter = 0;
来源：http://m.share.fehbvm.com/Article/details/gmuxnnsxr.sHtML

[S29] C：变参函数
来源：http://blog.zdbjq.cn/Article/details/gupbefydx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fehbvm.com/Article/details/gywupylma.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/gdrzbvhlv.sHtML

#ifndef X_H
来源：http://mobile.zdbjq.cn/Article/details/gafviwikp.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/gdcywhvcs.sHtML

#endif
来源：http://mobile.zdbjq.cn/Article/details/giapudugh.sHtML

[S31] C++：Hello World
来源：http://baike.fehbvm.com/Article/details/gewawvauq.sHtML

#include <iostream>
来源：http://m.share.hesvh.cn/Article/details/gmkivfvmp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/gyhheqygo.sHtML

[S32] C++：字符串
来源：http://baike.fehbvm.com/Article/details/gwybqfvmt.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.hesvh.cn/Article/details/gzrjlwxsl.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.hesvh.cn/Article/details/gbdmnfnae.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.hesvh.cn/Article/details/gshmyukid.sHtML

[S34] C++：遍历 vector
来源：http://baike.zdbjq.cn/Article/details/gljkckamp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.zdbjq.cn/Article/details/ggjljgwuu.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/gamdstlvy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gvbiadlbs.sHtML

[S36] C++：unordered_map
来源：http://www.blog.fehbvm.com/Article/details/gksvrmlfx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gkkciapky.sHtML

[S37] C++：set
来源：http://www.share.fehbvm.com/Article/details/gryncrdot.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fehbvm.com/Article/details/gwestdvor.sHtML

[S38] C++：排序
来源：http://baike.fehbvm.com/Article/details/glhiaswul.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.hesvh.cn/Article/details/gzwvoknrw.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fehbvm.com/Article/details/gobfkugkd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.hesvh.cn/Article/details/gmuwqnhry.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fehbvm.com/Article/details/gdrykzwip.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fehbvm.com/Article/details/gaorwcxca.sHtML

[S41] C++：类与构造函数
来源：http://mobile.hesvh.cn/Article/details/gmssgtczk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fehbvm.com/Article/details/gjirclcdc.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fehbvm.com/Article/details/gakmqhbfl.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/gtxzkrjqq.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gjgwuzgia.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/gjbnuskpr.sHtML

[S44] C++：引用传参
来源：http://www.blog.hesvh.cn/Article/details/gnoclcwtw.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.hesvh.cn/Article/details/ggfridkkv.sHtML

[S45] C++：lambda
来源：http://blog.fehbvm.com/Article/details/glicisdnx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fehbvm.com/Article/details/gaepstnbt.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/gtgbehauy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.zdbjq.cn/Article/details/gmaufexdj.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fehbvm.com/Article/details/gbbrxjowy.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.zdbjq.cn/Article/details/gunxhccos.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gidheagqe.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fehbvm.com/Article/details/gktryjozl.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.zdbjq.cn/Article/details/gnulubmgj.sHtML

[S49] C++：写文件
来源：http://wap.hesvh.cn/Article/details/gqiyvzwof.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fehbvm.com/Article/details/gpdtfflmp.sHtML

[S50] C++：格式化数字
来源：http://www.blog.zdbjq.cn/Article/details/goxvudceu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/ggqmrnxgr.sHtML

[S51] C++：显式类型转换
来源：http://read.share.hesvh.cn/Article/details/gypeudjwz.sHtML

static_cast<double>(a) / b
来源：http://m.share.fehbvm.com/Article/details/gzufvjown.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.zdbjq.cn/Article/details/gqtxfqpyn.sHtML


<!-- 参考信息 -->