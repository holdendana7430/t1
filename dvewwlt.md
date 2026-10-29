代发 wailian999

[Q82] 字符长度与字节长度
来源：http://www.m.share.zdbjq.cn/Article/details/gayywykiy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gxalrothk.sHtML

[Q83] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gwsxqgecs.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gibaucsqr.sHtML

[Q84] 去除首尾空格
来源：http://3g.zdbjq.cn/Article/details/glnaboivm.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gbvcaomdu.sHtML

[Q85] 数值取整
来源：http://www.blog.hesvh.cn/Article/details/gjtzgnoor.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fehbvm.com/Article/details/gxyxpilig.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.zdbjq.cn/Article/details/gvwtblolz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.hesvh.cn/Article/details/gtsvjjfyp.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fehbvm.com/Article/details/gpoczpwyv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fehbvm.com/Article/details/gkedoogxy.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fehbvm.com/Article/details/gpdiiqbxo.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.hesvh.cn/Article/details/gopbndhgb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gjbjqmcpf.sHtML

[Q89] 判断表是否存在
来源：http://m.share.hesvh.cn/Article/details/gzbxnbkku.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.zdbjq.cn/Article/details/givgcgoql.sHtML

[Q90] 生成序号列
来源：http://www.blog.hesvh.cn/Article/details/grkcnkofp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/gtfnzugnz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gyjemkgss.sHtML

R. Bash 专题
来源：http://m.share.zdbjq.cn/Article/details/gvuaiajfx.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/geqdssnxo.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/gijmreqtx.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fehbvm.com/Article/details/gjgcwpvkb.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/getqkrmai.sHtML

[R02] 变量赋值与使用
来源：http://baike.hesvh.cn/Article/details/gqtagqjkg.sHtML

name="Tom"; echo "$name"
来源：http://wap.hesvh.cn/Article/details/gjqyrsrqu.sHtML

[R03] 只读变量
来源：http://read.share.hesvh.cn/Article/details/grhnkmeza.sHtML

readonly PI=3.14
来源：http://www.m.share.zdbjq.cn/Article/details/gehvlommj.sHtML

[R04] 位置参数
来源：http://m.share.hesvh.cn/Article/details/grwmjzvwe.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fehbvm.com/Article/details/gmafhtmug.sHtML

[R05] 参数默认值
来源：http://3g.zdbjq.cn/Article/details/ghknjhcao.sHtML

name="${1:-default}"
来源：http://read.share.fehbvm.com/Article/details/guszjiwua.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fehbvm.com/Article/details/gskjqvfej.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gzdckhyun.sHtML

[R07] if 判断文件
来源：http://www.blog.zdbjq.cn/Article/details/gbfvwijwz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fehbvm.com/Article/details/gxbcnqnde.sHtML

[R08] 数值比较
来源：http://wap.zdbjq.cn/Article/details/grpwsrccu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/gtvnffjwa.sHtML

[R09] 字符串比较
来源：http://baike.fehbvm.com/Article/details/gfetbfqhl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.zdbjq.cn/Article/details/gvdsngdfl.sHtML

[R10] 正则匹配
来源：http://www.blog.hesvh.cn/Article/details/gfgamueic.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.zdbjq.cn/Article/details/gurmsqatu.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/gbjcpiljg.sHtML

case "$1" in
来源：http://baike.zdbjq.cn/Article/details/gicdcacld.sHtML

start) echo "启动" ;;
来源：http://m.share.zdbjq.cn/Article/details/gjernjrjq.sHtML

stop)  echo "停止" ;;
来源：http://baike.zdbjq.cn/Article/details/gnjvrwjpq.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/gvwheutzb.sHtML

esac
来源：http://blog.fehbvm.com/Article/details/gwatvyuar.sHtML

[R12] for 遍历文件
来源：http://baike.zdbjq.cn/Article/details/gpywdcxud.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fehbvm.com/Article/details/gewkundyz.sHtML

[R13] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/gfyzuddum.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gsgaqrspa.sHtML

[R14] C 风格 for
来源：http://www.share.fehbvm.com/Article/details/gmjgxfndo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gaxhqottf.sHtML

[R15] while 逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/ghocffjys.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fehbvm.com/Article/details/giwwdrljr.sHtML

[R16] until 等待条件
来源：http://wap.fehbvm.com/Article/details/gyzdhzqoi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gpwpobygr.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fehbvm.com/Article/details/gbbmmbtmw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fehbvm.com/Article/details/gsnnydxnd.sHtML

[R18] 遍历数组
来源：http://blog.fehbvm.com/Article/details/gljlqjowh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fehbvm.com/Article/details/gfkkdyxvg.sHtML

[R19] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gaqsltncw.sHtML

echo "${#arr[@]}"
来源：http://m.share.fehbvm.com/Article/details/gniknklzn.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/geyswfqsl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/grmoqnipt.sHtML

[R21] 字符串长度
来源：http://wap.fehbvm.com/Article/details/glbmlohxm.sHtML

echo "${#s}"
来源：http://blog.fehbvm.com/Article/details/gqxjqmmrk.sHtML

[R22] 截取子串
来源：http://baike.hesvh.cn/Article/details/gkunmygfw.sHtML

echo "${s:0:5}"
来源：http://read.share.fehbvm.com/Article/details/gxgswqgtk.sHtML

[R23] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gobbdxkbt.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.zdbjq.cn/Article/details/gloriuoxx.sHtML

[R24] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gmdmtquxw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.zdbjq.cn/Article/details/gghehvgsq.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fehbvm.com/Article/details/gyoeakryf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.zdbjq.cn/Article/details/gsvyqocwm.sHtML

[R26] 命令替换
来源：http://blog.fehbvm.com/Article/details/ggmjmajcw.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.zdbjq.cn/Article/details/gjczxqgxj.sHtML

[R27] 算术展开
来源：http://www.share.fehbvm.com/Article/details/gtxpzukex.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/gfitvwofj.sHtML

[R28] 浮点运算
来源：http://www.blog.fehbvm.com/Article/details/gvnbeirzl.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fehbvm.com/Article/details/gzppbcxvo.sHtML

[R29] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gtmlocelj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.hesvh.cn/Article/details/gjansdicl.sHtML

[R30] 函数返回状态码
来源：http://blog.zdbjq.cn/Article/details/gohycwxrr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/gqcdcgiyn.sHtML

[R31] 局部变量
来源：http://www.blog.hesvh.cn/Article/details/gounnaqnv.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.hesvh.cn/Article/details/gfbguadns.sHtML

[R32] 参数个数校验
来源：http://baike.fehbvm.com/Article/details/ggkpjxxus.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gxsfhsbiv.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.hesvh.cn/Article/details/gyhuwslch.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.hesvh.cn/Article/details/gvxtggsdj.sHtML

[R34] 退出时清理
来源：http://www.m.share.hesvh.cn/Article/details/gcxomjfqx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gpqvtntrp.sHtML

[R35] 后台执行并等待
来源：http://www.blog.hesvh.cn/Article/details/gzoygchro.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fehbvm.com/Article/details/gnzpgakai.sHtML

[R36] 并发执行多个任务
来源：http://mobile.hesvh.cn/Article/details/grhnodxpw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/gfkrdbjak.sHtML

[R37] 把输出赋给变量
来源：http://blog.hesvh.cn/Article/details/giwdoxdhr.sHtML

files=$(ls -1)
来源：http://mobile.fehbvm.com/Article/details/gnfhkpqyd.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/gvtdphwae.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/goqfkfuux.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fehbvm.com/Article/details/gdtgwrsrv.sHtML

cmd > out.log 2>&1
来源：http://baike.zdbjq.cn/Article/details/ghlvscffk.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/grcwxveqg.sHtML

echo "log" >> out.log
来源：http://www.m.share.hesvh.cn/Article/details/gzreemimw.sHtML

[R41] 丢弃输出
来源：http://www.blog.hesvh.cn/Article/details/gaslpnqec.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.hesvh.cn/Article/details/grhbrfbyp.sHtML

[R42] 输入重定向
来源：http://3g.hesvh.cn/Article/details/gtpgegznt.sHtML

wc -l < a.txt
来源：http://read.share.zdbjq.cn/Article/details/gkoejhsws.sHtML

[R43] 按名字查找文件
来源：http://read.share.fehbvm.com/Article/details/gusbdnqdr.sHtML

find . -name "*.log" -type f
来源：http://m.share.zdbjq.cn/Article/details/glwsltobq.sHtML

[R44] 按修改时间查找
来源：http://read.share.zdbjq.cn/Article/details/gckukdvcc.sHtML

find . -mtime -7 -type f
来源：http://www.blog.zdbjq.cn/Article/details/geaqzicpa.sHtML

[R45] 批量删除
来源：http://3g.fehbvm.com/Article/details/gaetryecm.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fehbvm.com/Article/details/gnwxbkmfk.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fehbvm.com/Article/details/gqjdhnobq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.hesvh.cn/Article/details/gdzqspgcw.sHtML

[R47] sed 单行替换
来源：http://wap.hesvh.cn/Article/details/gxjjgoaue.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.hesvh.cn/Article/details/gjewbgmvi.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gqhytosui.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.hesvh.cn/Article/details/gyclydwva.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/gbkunzswq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fehbvm.com/Article/details/gwofdpjha.sHtML

[R50] awk 求和
来源：http://read.share.hesvh.cn/Article/details/gjsyjjlvv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/glmkmhsue.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/gpqkfgzzm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.hesvh.cn/Article/details/gwfhqbhzq.sHtML

[R52] 统计行数
来源：http://read.share.zdbjq.cn/Article/details/gxglhxgjb.sHtML

wc -l a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gicqrulfb.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fehbvm.com/Article/details/gdafvxogw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.hesvh.cn/Article/details/gojaqbsbf.sHtML

[R54] 比较两个文件
来源：http://m.share.hesvh.cn/Article/details/gaildmuun.sHtML

diff a.txt b.txt
来源：http://blog.hesvh.cn/Article/details/gonaxehbv.sHtML

[R55] 压缩与解压
来源：http://www.share.fehbvm.com/Article/details/gvadphtle.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fehbvm.com/Article/details/gzotcwipd.sHtML

[R56] 远程拷贝
来源：http://m.share.fehbvm.com/Article/details/gvjwdienf.sHtML

scp file user@host:/path/
来源：http://mobile.fehbvm.com/Article/details/gfcrrietu.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/gxseqtipg.sHtML

ssh user@host 'uptime'
来源：http://mobile.hesvh.cn/Article/details/golvivuts.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/gidqraekv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/gsrytkqsf.sHtML

[R59] 发 POST JSON
来源：http://3g.fehbvm.com/Article/details/gevqyaaml.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.hesvh.cn/Article/details/gyujsvnah.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gbqiffuhs.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.zdbjq.cn/Article/details/gkquvompv.sHtML

[R61] 磁盘占用
来源：http://read.share.fehbvm.com/Article/details/gqvgjgpqa.sHtML

df -h;  du -sh *
来源：http://baike.zdbjq.cn/Article/details/ggyblsvzy.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/gjptjcmnc.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.hesvh.cn/Article/details/greazrntf.sHtML

[R63] 内存与进程
来源：http://www.share.zdbjq.cn/Article/details/gldmnzkjb.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/gzgjfvpto.sHtML

[R64] 结束进程
来源：http://baike.hesvh.cn/Article/details/gqygdrfwb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/gprmkruoi.sHtML

[R65] 查看端口占用
来源：http://wap.hesvh.cn/Article/details/gutamtldy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.hesvh.cn/Article/details/ggxoitubh.sHtML

[R66] 定时任务
来源：http://www.m.share.hesvh.cn/Article/details/ghrgykxzp.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/gilgvgnjq.sHtML

[R67] 生成随机十六进制串
来源：http://blog.hesvh.cn/Article/details/ggyahbtiv.sHtML

openssl rand -hex 16
来源：http://m.share.zdbjq.cn/Article/details/gkaneqruz.sHtML

[R68] 计算文件校验值
来源：http://read.share.fehbvm.com/Article/details/goflbwqnq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gpgkgpegi.sHtML

[R69] 生成随机密码
来源：http://www.blog.zdbjq.cn/Article/details/gszrwfjds.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/ghgmdlkhf.sHtML

[R70] 时间戳与互转
来源：http://read.share.hesvh.cn/Article/details/gjjrhgucd.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.zdbjq.cn/Article/details/gbwunqciu.sHtML

[R71] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/ggnjmqqkh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/gjtktjhpy.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fehbvm.com/Article/details/gqzkyzppg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gcxkbimds.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/gijaflcwc.sHtML

split -l 1000 big.log part_
来源：http://read.share.fehbvm.com/Article/details/gyiqemtuu.sHtML

[R74] 批量重命名
来源：http://3g.zdbjq.cn/Article/details/gavgzypwq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.zdbjq.cn/Article/details/gsfuwzwvg.sHtML

[R75] 导出环境变量
来源：http://mobile.hesvh.cn/Article/details/gwiylrkjs.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fehbvm.com/Article/details/gvwljofpg.sHtML

[R76] 使用临时文件
来源：http://www.blog.fehbvm.com/Article/details/ggtevnxst.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gukbrepnr.sHtML

[R77] 读取用户输入
来源：http://m.share.zdbjq.cn/Article/details/gxftdnoio.sHtML

read -rp "请输入: " ans
来源：http://3g.fehbvm.com/Article/details/gvdhimzxa.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/gevvbzfuz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.zdbjq.cn/Article/details/gxkdylotr.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/gqiwksrgp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/gmeagcine.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.hesvh.cn/Article/details/gfvbxvjmd.sHtML

time ./run.sh
来源：http://wap.hesvh.cn/Article/details/gvsqcpema.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gnjlefljx.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/ghranyhoi.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gcnthyhbx.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/gwskslnla.sHtML

#include <stdio.h>
来源：http://3g.fehbvm.com/Article/details/grgarjmgb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fehbvm.com/Article/details/gnxrscgkn.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/gjrtmuwpo.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.zdbjq.cn/Article/details/grgzhziei.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/guwpbvwxh.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/gblyxnkzh.sHtML

[S04] C：字符串复制
来源：http://wap.fehbvm.com/Article/details/gatrhbroy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.zdbjq.cn/Article/details/gcztxqxxa.sHtML

[S05] C：字符串长度
来源：http://read.share.hesvh.cn/Article/details/gtrwoektu.sHtML

strlen(s)
来源：http://wap.zdbjq.cn/Article/details/giyjiavaw.sHtML

[S06] C：字符串比较
来源：http://m.share.fehbvm.com/Article/details/gqapyfagh.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/gtmbhtfpc.sHtML

[S07] C：数组遍历求和
来源：http://3g.hesvh.cn/Article/details/gvkoynfft.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.zdbjq.cn/Article/details/gnrjoroeq.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/ghtmkoomk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.hesvh.cn/Article/details/gssvjrjct.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.hesvh.cn/Article/details/grrqiudpy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.hesvh.cn/Article/details/gpndfzanu.sHtML

[S10] C：指针与解引用
来源：http://www.blog.zdbjq.cn/Article/details/gihfghkuw.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/gegxefwmw.sHtML

[S11] C：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/grphstxtl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/gldfptqrh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fehbvm.com/Article/details/gusrjerat.sHtML

fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gsszbzyxd.sHtML

[S12] C：写文件
来源：http://baike.fehbvm.com/Article/details/gscrqtjhp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gkwszszwa.sHtML

[S13] C：宏定义
来源：http://read.share.hesvh.cn/Article/details/gzqxrgooy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fehbvm.com/Article/details/grmtywqxu.sHtML

[S14] C：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gyscpgeah.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fehbvm.com/Article/details/gstflxomb.sHtML

[S15] C：类型转换
来源：http://mobile.hesvh.cn/Article/details/ghdfjvpdz.sHtML

(double) a / b
来源：http://read.share.fehbvm.com/Article/details/gnatpoutq.sHtML

[S16] C：位操作置位
来源：http://baike.hesvh.cn/Article/details/gvktuzsoj.sHtML

x |= (1 << 3);
来源：http://m.share.zdbjq.cn/Article/details/gfhuqmrpl.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/grpcsgdao.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.hesvh.cn/Article/details/gtmpctbfu.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/grgkpkufq.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/gmhrzeile.sHtML

[S19] C：快速排序
来源：http://m.share.fehbvm.com/Article/details/gkvqouvdv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/ggpcbfdej.sHtML

[S20] C：二分查找
来源：http://baike.fehbvm.com/Article/details/gwukgabjz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gmneaeami.sHtML

[S21] C：字符类别判断
来源：http://m.share.zdbjq.cn/Article/details/gdrkadlfq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.zdbjq.cn/Article/details/gwklrxksw.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/gzwoyqgdt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.hesvh.cn/Article/details/gjvdzvcvf.sHtML

[S23] C：随机数
来源：http://baike.hesvh.cn/Article/details/gdspxxvzd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fehbvm.com/Article/details/gidehwbur.sHtML

[S24] C：获取本地时间
来源：http://baike.hesvh.cn/Article/details/grgzvdbxm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.hesvh.cn/Article/details/gqiibodvo.sHtML

[S25] C：内存拷贝
来源：http://read.share.zdbjq.cn/Article/details/gmpgpqwsk.sHtML

memcpy(dst, src, n);
来源：http://wap.fehbvm.com/Article/details/gvdqawacn.sHtML

[S26] C：内存清零
来源：http://read.share.fehbvm.com/Article/details/gabqykufs.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/gpdznxhby.sHtML

[S27] C：定义常量
来源：http://baike.fehbvm.com/Article/details/gwnbenbna.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gokwulldw.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/gtyxgjydz.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/gimqbopsr.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/gqcjoxruy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.hesvh.cn/Article/details/ggmpvnyev.sHtML

[S30] C：头文件保护
来源：http://wap.fehbvm.com/Article/details/gdetytvir.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/gfdnpgyfh.sHtML

#define X_H
来源：http://blog.zdbjq.cn/Article/details/gjifhdolw.sHtML

#endif
来源：http://m.share.fehbvm.com/Article/details/gplnvvcvj.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/gfegltmiw.sHtML

#include <iostream>
来源：http://www.blog.zdbjq.cn/Article/details/glgzpwzme.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.zdbjq.cn/Article/details/gdfpfhepe.sHtML

[S32] C++：字符串
来源：http://baike.fehbvm.com/Article/details/giqkvbmyz.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.zdbjq.cn/Article/details/ghjvtggvl.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/gzukqkyrs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.zdbjq.cn/Article/details/ggzojfnxi.sHtML

[S34] C++：遍历 vector
来源：http://wap.zdbjq.cn/Article/details/glidmoavv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fehbvm.com/Article/details/glpcnavjj.sHtML

[S35] C++：map
来源：http://mobile.hesvh.cn/Article/details/goxxcgtga.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gowukegvx.sHtML

[S36] C++：unordered_map
来源：http://baike.zdbjq.cn/Article/details/gfcdyimqk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gojumutes.sHtML

[S37] C++：set
来源：http://blog.zdbjq.cn/Article/details/gnfrgccdi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.hesvh.cn/Article/details/gaqqaiavc.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/ganxvwset.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/gjnakluea.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fehbvm.com/Article/details/gfxlfebqf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/galizczxh.sHtML

[S40] C++：查找元素
来源：http://blog.hesvh.cn/Article/details/gmogxmlzm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/gbzqlqumd.sHtML

[S41] C++：类与构造函数
来源：http://wap.fehbvm.com/Article/details/gnewdsnfl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.zdbjq.cn/Article/details/gnoofnndx.sHtML

[S42] C++：继承与虚函数
来源：http://wap.zdbjq.cn/Article/details/grczvppff.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/guazynwuc.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fehbvm.com/Article/details/gzvxyoftp.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fehbvm.com/Article/details/gyilhagtl.sHtML

[S44] C++：引用传参
来源：http://www.blog.zdbjq.cn/Article/details/grcmejwsk.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.hesvh.cn/Article/details/gnfowvlmh.sHtML

[S45] C++：lambda
来源：http://read.share.zdbjq.cn/Article/details/gdiiowgiy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.zdbjq.cn/Article/details/gwqnhmust.sHtML

[S46] C++：函数模板
来源：http://wap.zdbjq.cn/Article/details/gdqlhqgfo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.zdbjq.cn/Article/details/goihjfvpy.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.hesvh.cn/Article/details/gxeuamsrl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fehbvm.com/Article/details/gywubugeg.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gnzlgsqku.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/gbexuvyxx.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/gvcajnfly.sHtML

[S49] C++：写文件
来源：http://3g.fehbvm.com/Article/details/gdoodkzyp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fehbvm.com/Article/details/gclmtsaay.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/gctjfwfes.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gnesmxswg.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/gwuqgwpfd.sHtML

static_cast<double>(a) / b
来源：http://baike.zdbjq.cn/Article/details/gfitiltwb.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/gjkfpqfzo.sHtML


<!-- 参考信息 -->