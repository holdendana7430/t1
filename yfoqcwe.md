代发 wailian999

[Q82] 字符长度与字节长度
来源：http://www.m.share.zdbjq.cn/Article/details/gwoeyowne.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gktmymkdv.sHtML

[Q83] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gepgxkaao.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/grqdeaxac.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fehbvm.com/Article/details/ghtrdynzd.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gitdluals.sHtML

[Q85] 数值取整
来源：http://3g.fehbvm.com/Article/details/gbhjyfudr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.hesvh.cn/Article/details/gqcebiwme.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.zdbjq.cn/Article/details/gcfkiegpe.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.hesvh.cn/Article/details/gcioxbncx.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fehbvm.com/Article/details/ghzuxhpci.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fehbvm.com/Article/details/glwrxqxfd.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.zdbjq.cn/Article/details/gumvijtsv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.hesvh.cn/Article/details/gkffferhc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.hesvh.cn/Article/details/gtujuztjj.sHtML

[Q89] 判断表是否存在
来源：http://m.share.zdbjq.cn/Article/details/gesnvcdlt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.hesvh.cn/Article/details/glypxefah.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/gekmyvbfh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.zdbjq.cn/Article/details/gvnhetohx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmislgtxi.sHtML

R. Bash 专题
来源：http://wap.hesvh.cn/Article/details/gzqrsieyz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzeusskey.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/gaoavpdru.sHtML

#!/usr/bin/env bash
来源：http://www.blog.zdbjq.cn/Article/details/gaqfezxyg.sHtML

set -euo pipefail
来源：http://mobile.zdbjq.cn/Article/details/gjdtxeovc.sHtML

[R02] 变量赋值与使用
来源：http://baike.zdbjq.cn/Article/details/gqckuhhek.sHtML

name="Tom"; echo "$name"
来源：http://m.share.zdbjq.cn/Article/details/gutccytdk.sHtML

[R03] 只读变量
来源：http://blog.hesvh.cn/Article/details/gbrewhhzx.sHtML

readonly PI=3.14
来源：http://m.share.zdbjq.cn/Article/details/gxwozbnla.sHtML

[R04] 位置参数
来源：http://read.share.fehbvm.com/Article/details/gubkyadoj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fehbvm.com/Article/details/gdkukuhyz.sHtML

[R05] 参数默认值
来源：http://www.share.hesvh.cn/Article/details/gfeowzgfd.sHtML

name="${1:-default}"
来源：http://www.m.share.zdbjq.cn/Article/details/gdkrgkdsc.sHtML

[R06] 判断命令是否存在
来源：http://read.share.zdbjq.cn/Article/details/gotqnufqw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gxrcvsnxc.sHtML

[R07] if 判断文件
来源：http://mobile.hesvh.cn/Article/details/gzxjdypsw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fehbvm.com/Article/details/ghxekyzrm.sHtML

[R08] 数值比较
来源：http://www.m.share.hesvh.cn/Article/details/guakdxhds.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.zdbjq.cn/Article/details/gbxhzgeel.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/gtqcxstup.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.hesvh.cn/Article/details/guqptsvqs.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gxemubtww.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fehbvm.com/Article/details/gulythyvj.sHtML

[R11] case 多分支
来源：http://wap.zdbjq.cn/Article/details/gartenvll.sHtML

case "$1" in
来源：http://wap.zdbjq.cn/Article/details/gfxhqkwei.sHtML

start) echo "启动" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gxymczyin.sHtML

stop)  echo "停止" ;;
来源：http://read.share.zdbjq.cn/Article/details/gxelyfrba.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fehbvm.com/Article/details/geyaxpfeg.sHtML

esac
来源：http://www.share.fehbvm.com/Article/details/gazooylon.sHtML

[R12] for 遍历文件
来源：http://www.blog.zdbjq.cn/Article/details/glwtzfppy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fehbvm.com/Article/details/ghtnxhcnq.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/gqooluedg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gttzfcoif.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/gfqqncyaz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/guupwdkok.sHtML

[R15] while 逐行读文件
来源：http://baike.hesvh.cn/Article/details/gsajoloib.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.hesvh.cn/Article/details/gljpynvqv.sHtML

[R16] until 等待条件
来源：http://m.share.zdbjq.cn/Article/details/glpztlzec.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/glrcdkdsq.sHtML

[R17] 数组定义与取值
来源：http://www.share.zdbjq.cn/Article/details/gqkprmohj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.hesvh.cn/Article/details/gtvomdyxa.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gptzyyzpt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gsfsqknka.sHtML

[R19] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gjbdhvsqa.sHtML

echo "${#arr[@]}"
来源：http://read.share.fehbvm.com/Article/details/gqlnmllro.sHtML

[R20] 关联数组（字典）
来源：http://read.share.hesvh.cn/Article/details/goubhdkuy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/glnkuoxzl.sHtML

[R21] 字符串长度
来源：http://mobile.fehbvm.com/Article/details/gqxujphjd.sHtML

echo "${#s}"
来源：http://wap.fehbvm.com/Article/details/gjnrohdos.sHtML

[R22] 截取子串
来源：http://3g.fehbvm.com/Article/details/gaintenji.sHtML

echo "${s:0:5}"
来源：http://m.share.zdbjq.cn/Article/details/ghyprirmc.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gtuafyoww.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/gzosjxjyg.sHtML

[R24] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gsqpgdhza.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fehbvm.com/Article/details/gayruvkzm.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fehbvm.com/Article/details/grsmxzohb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fehbvm.com/Article/details/gztjsdxbq.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/ggxjgaoax.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/gkmfnytxs.sHtML

[R27] 算术展开
来源：http://m.share.hesvh.cn/Article/details/gmrqzrygt.sHtML

echo $((1 + 2 * 3))
来源：http://wap.hesvh.cn/Article/details/guzhdzwyg.sHtML

[R28] 浮点运算
来源：http://mobile.zdbjq.cn/Article/details/glvupnlxc.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fehbvm.com/Article/details/glanotamq.sHtML

[R29] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gzidhrsht.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fehbvm.com/Article/details/gcsbghymq.sHtML

[R30] 函数返回状态码
来源：http://baike.zdbjq.cn/Article/details/gwxnvqrmu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.zdbjq.cn/Article/details/gbhkhfbhh.sHtML

[R31] 局部变量
来源：http://mobile.zdbjq.cn/Article/details/gjiuzoaud.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/glezhxvun.sHtML

[R32] 参数个数校验
来源：http://www.m.share.zdbjq.cn/Article/details/gcmhsikhj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gjvpyiyiz.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.zdbjq.cn/Article/details/gekwrkfho.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/gneapvfgu.sHtML

[R34] 退出时清理
来源：http://blog.fehbvm.com/Article/details/gpnipxvvo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gxtxbvgtq.sHtML

[R35] 后台执行并等待
来源：http://read.share.hesvh.cn/Article/details/gcqebjhpl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.hesvh.cn/Article/details/gxnkqoedj.sHtML

[R36] 并发执行多个任务
来源：http://3g.fehbvm.com/Article/details/gvcdaratb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/gqzcrdvpk.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.zdbjq.cn/Article/details/gexkmvzpq.sHtML

files=$(ls -1)
来源：http://www.blog.zdbjq.cn/Article/details/gtylzkkfz.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/gpryaulpi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.hesvh.cn/Article/details/gurlcavvh.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fehbvm.com/Article/details/gplmnakgl.sHtML

cmd > out.log 2>&1
来源：http://blog.hesvh.cn/Article/details/gcwoiofnk.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/gimhhqfek.sHtML

echo "log" >> out.log
来源：http://mobile.fehbvm.com/Article/details/gmzqsbajn.sHtML

[R41] 丢弃输出
来源：http://www.m.share.zdbjq.cn/Article/details/gtltttipo.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/ggvgfjdln.sHtML

[R42] 输入重定向
来源：http://3g.hesvh.cn/Article/details/guivgmbvc.sHtML

wc -l < a.txt
来源：http://www.blog.hesvh.cn/Article/details/gqdaupwfi.sHtML

[R43] 按名字查找文件
来源：http://baike.zdbjq.cn/Article/details/gsbpimcwq.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.hesvh.cn/Article/details/grntxtrxt.sHtML

[R44] 按修改时间查找
来源：http://mobile.hesvh.cn/Article/details/gjhabohtz.sHtML

find . -mtime -7 -type f
来源：http://www.blog.zdbjq.cn/Article/details/gmvexqrrq.sHtML

[R45] 批量删除
来源：http://www.m.share.fehbvm.com/Article/details/gozrgotcl.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fehbvm.com/Article/details/gxspzhcdo.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fehbvm.com/Article/details/goaejihbu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.zdbjq.cn/Article/details/gykxssiyt.sHtML

[R47] sed 单行替换
来源：http://www.share.fehbvm.com/Article/details/gunkiyqfr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gvygmcmxf.sHtML

[R48] awk 取指定列
来源：http://www.share.zdbjq.cn/Article/details/gpntfrxil.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.zdbjq.cn/Article/details/grvfewjvc.sHtML

[R49] awk 带条件
来源：http://m.share.zdbjq.cn/Article/details/ggyzifrrs.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/gdnlmdenf.sHtML

[R50] awk 求和
来源：http://3g.fehbvm.com/Article/details/ggqbvkwtx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.zdbjq.cn/Article/details/guzsafjhf.sHtML

[R51] 排序去重取前几
来源：http://blog.hesvh.cn/Article/details/gzremowyj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/gmkajkmky.sHtML

[R52] 统计行数
来源：http://baike.zdbjq.cn/Article/details/gndjusxjv.sHtML

wc -l a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gvdiftiut.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.zdbjq.cn/Article/details/ghyjqpwfx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.zdbjq.cn/Article/details/ggjrugnli.sHtML

[R54] 比较两个文件
来源：http://www.share.fehbvm.com/Article/details/ghosettub.sHtML

diff a.txt b.txt
来源：http://mobile.zdbjq.cn/Article/details/gqknkjezi.sHtML

[R55] 压缩与解压
来源：http://m.share.hesvh.cn/Article/details/ghwotnfua.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fehbvm.com/Article/details/gvxgsezjz.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/gdjwvyeym.sHtML

scp file user@host:/path/
来源：http://www.share.fehbvm.com/Article/details/gyviyehfe.sHtML

[R57] 远程执行命令
来源：http://www.m.share.zdbjq.cn/Article/details/gzzwrwjst.sHtML

ssh user@host 'uptime'
来源：http://m.share.fehbvm.com/Article/details/gveouiwhm.sHtML

[R58] 下载文件
来源：http://baike.fehbvm.com/Article/details/gumkokgzt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.zdbjq.cn/Article/details/gomgwmzot.sHtML

[R59] 发 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gigqynzhz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.zdbjq.cn/Article/details/glcopxhqy.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gjuysdyhd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.zdbjq.cn/Article/details/gnasrmjle.sHtML

[R61] 磁盘占用
来源：http://wap.hesvh.cn/Article/details/gkldenymh.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/gtppvmkmt.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fehbvm.com/Article/details/guxknorcz.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.hesvh.cn/Article/details/gmtmvmmou.sHtML

[R63] 内存与进程
来源：http://m.share.zdbjq.cn/Article/details/gnrwpwiui.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/ghdoeohfu.sHtML

[R64] 结束进程
来源：http://wap.zdbjq.cn/Article/details/gbmgqoqwm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.zdbjq.cn/Article/details/gzbkelefk.sHtML

[R65] 查看端口占用
来源：http://baike.zdbjq.cn/Article/details/gmiwuxgcd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.hesvh.cn/Article/details/ghtemnver.sHtML

[R66] 定时任务
来源：http://3g.zdbjq.cn/Article/details/glusvenkp.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/gfvzjlyjq.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.zdbjq.cn/Article/details/gbckfcgfr.sHtML

openssl rand -hex 16
来源：http://blog.zdbjq.cn/Article/details/gcpqqqbgk.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/gcwduznct.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.hesvh.cn/Article/details/gprltndoq.sHtML

[R69] 生成随机密码
来源：http://wap.hesvh.cn/Article/details/guqkpofuj.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/gzyindzgm.sHtML

[R70] 时间戳与互转
来源：http://3g.zdbjq.cn/Article/details/gxkfzelfq.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/gmtxfyhpz.sHtML

[R71] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gmamijras.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/gidntkrwp.sHtML

[R72] 等待端口就绪
来源：http://3g.fehbvm.com/Article/details/gziulejmi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gvmjtwucp.sHtML

[R73] 分割大日志
来源：http://mobile.fehbvm.com/Article/details/glkygmqim.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/gozcthebd.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/gqwkdflak.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fehbvm.com/Article/details/gcbgubeqr.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/gwqwdgthi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.hesvh.cn/Article/details/gxwcbdkld.sHtML

[R76] 使用临时文件
来源：http://mobile.zdbjq.cn/Article/details/gubzhyjls.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gtltkicaq.sHtML

[R77] 读取用户输入
来源：http://wap.hesvh.cn/Article/details/ggoaoohsa.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fehbvm.com/Article/details/gccxxppqf.sHtML

[R78] 交互式菜单
来源：http://www.m.share.hesvh.cn/Article/details/gklyfqtnf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.hesvh.cn/Article/details/genrehebb.sHtML

[R79] 解析命令行选项
来源：http://m.share.fehbvm.com/Article/details/gxtekfinq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.hesvh.cn/Article/details/gvyavgaqu.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/gljvsuagu.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/gyzknmxnp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gtyvjuiml.sHtML

S. C / C++ 专题
来源：http://m.share.fehbvm.com/Article/details/gtvnlfqkt.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ggoootifx.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/gkolkopms.sHtML

#include <stdio.h>
来源：http://mobile.hesvh.cn/Article/details/gqljczhfc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.hesvh.cn/Article/details/ghycspmkn.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.hesvh.cn/Article/details/gijvumqlj.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fehbvm.com/Article/details/grqzpjwfi.sHtML

[S03] C：读入整数
来源：http://3g.hesvh.cn/Article/details/gxjmimubo.sHtML

int x; scanf("%d", &x);
来源：http://www.share.hesvh.cn/Article/details/gxbrduube.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/gmyirwehq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fehbvm.com/Article/details/gutjvoffp.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gfksfrmor.sHtML

strlen(s)
来源：http://mobile.hesvh.cn/Article/details/ggbtjpkoi.sHtML

[S06] C：字符串比较
来源：http://m.share.hesvh.cn/Article/details/gwoxnodnl.sHtML

strcmp(a, b) == 0
来源：http://blog.fehbvm.com/Article/details/gdlamefxc.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/gpkgjpxxg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/gynscajen.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.zdbjq.cn/Article/details/grkbxxgqs.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fehbvm.com/Article/details/gmefehyzp.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.hesvh.cn/Article/details/gdzgsofhq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gswokjwdt.sHtML

[S10] C：指针与解引用
来源：http://www.share.zdbjq.cn/Article/details/goulrbxat.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fehbvm.com/Article/details/gmjtgnzxl.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gxwihsszl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.hesvh.cn/Article/details/gdrskwstj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.zdbjq.cn/Article/details/gbmcyixzv.sHtML

fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gnoyckuuu.sHtML

[S12] C：写文件
来源：http://3g.hesvh.cn/Article/details/gfhpkgbff.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.hesvh.cn/Article/details/getjlvzhx.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/gmnyyjzog.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.hesvh.cn/Article/details/gvuwkfmlt.sHtML

[S14] C：枚举
来源：http://blog.hesvh.cn/Article/details/ggqyccjmc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fehbvm.com/Article/details/gyqeozigy.sHtML

[S15] C：类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gvazbgjco.sHtML

(double) a / b
来源：http://read.share.zdbjq.cn/Article/details/gmxwezqbr.sHtML

[S16] C：位操作置位
来源：http://m.share.fehbvm.com/Article/details/gsczbbnss.sHtML

x |= (1 << 3);
来源：http://www.blog.zdbjq.cn/Article/details/gvffmbffp.sHtML

[S17] C：安全拼接字符串
来源：http://3g.hesvh.cn/Article/details/gfmrgnxpq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.hesvh.cn/Article/details/gkhgiilak.sHtML

[S18] C：命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gbgvjstxx.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/gyratoiii.sHtML

[S19] C：快速排序
来源：http://m.share.hesvh.cn/Article/details/gkzygunuq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/goeatdghz.sHtML

[S20] C：二分查找
来源：http://m.share.fehbvm.com/Article/details/gjqzjfcit.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gpdtgakbf.sHtML

[S21] C：字符类别判断
来源：http://mobile.fehbvm.com/Article/details/gzugzznce.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.zdbjq.cn/Article/details/gyvliuheo.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gwfgglsjg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.hesvh.cn/Article/details/guxoxlcau.sHtML

[S23] C：随机数
来源：http://www.m.share.fehbvm.com/Article/details/gzxowpnkw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.zdbjq.cn/Article/details/giyuwfjkd.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/gdnxddoeb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.zdbjq.cn/Article/details/ghzftidwy.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/gdyhrordt.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/gporauswz.sHtML

[S26] C：内存清零
来源：http://www.blog.zdbjq.cn/Article/details/gcvdxqucn.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/gbdkfkonp.sHtML

[S27] C：定义常量
来源：http://read.share.hesvh.cn/Article/details/gjwpgsxoh.sHtML

const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gahozhwgl.sHtML

[S28] C：静态变量
来源：http://m.share.zdbjq.cn/Article/details/gatgiafgw.sHtML

static int counter = 0;
来源：http://mobile.fehbvm.com/Article/details/gfxvimwee.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/gijzxtgwq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.hesvh.cn/Article/details/gwmdmwtnt.sHtML

[S30] C：头文件保护
来源：http://m.share.hesvh.cn/Article/details/gzfltemwe.sHtML

#ifndef X_H
来源：http://read.share.hesvh.cn/Article/details/gjyksdvqw.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/gptotjhan.sHtML

#endif
来源：http://blog.hesvh.cn/Article/details/gyyekhzah.sHtML

[S31] C++：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gumtncssd.sHtML

#include <iostream>
来源：http://mobile.zdbjq.cn/Article/details/gpbzpkxst.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/gufgyagyp.sHtML

[S32] C++：字符串
来源：http://wap.hesvh.cn/Article/details/gtcetuehy.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.zdbjq.cn/Article/details/gugszjhee.sHtML

[S33] C++：vector 增删
来源：http://blog.fehbvm.com/Article/details/gdudgybad.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/gidminjhi.sHtML

[S34] C++：遍历 vector
来源：http://www.share.zdbjq.cn/Article/details/gctvpqggc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fehbvm.com/Article/details/gwehvibwy.sHtML

[S35] C++：map
来源：http://3g.zdbjq.cn/Article/details/gruukgzjh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gvvbwzzlk.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/ghcalhrai.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gojpijjyr.sHtML

[S37] C++：set
来源：http://blog.zdbjq.cn/Article/details/gkoydkrdu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.hesvh.cn/Article/details/gvnqmbkqk.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/gczztecqe.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.hesvh.cn/Article/details/gzkumooru.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.zdbjq.cn/Article/details/gfpshneac.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.zdbjq.cn/Article/details/gzofrjkvr.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/gyiybuefw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fehbvm.com/Article/details/gcwsvssso.sHtML

[S41] C++：类与构造函数
来源：http://mobile.hesvh.cn/Article/details/gccetgyir.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/gbygwbgzd.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fehbvm.com/Article/details/gaxgteshk.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fehbvm.com/Article/details/goxqzgcpu.sHtML

[S43] C++：智能指针
来源：http://www.blog.zdbjq.cn/Article/details/ghwgroyzt.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/gvpomoebh.sHtML

[S44] C++：引用传参
来源：http://mobile.zdbjq.cn/Article/details/gkfxdpxes.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.hesvh.cn/Article/details/grnegatpp.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/gstehbsoc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fehbvm.com/Article/details/gqecqvtvj.sHtML

[S46] C++：函数模板
来源：http://read.share.zdbjq.cn/Article/details/gobsyyiyl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fehbvm.com/Article/details/grmamyptg.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fehbvm.com/Article/details/glhqvjbcs.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.zdbjq.cn/Article/details/gaquhkatv.sHtML

[S48] C++：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gjpuvyqfn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/groygtiiv.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/gywvtklvn.sHtML

[S49] C++：写文件
来源：http://www.blog.fehbvm.com/Article/details/gqlbzyyke.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fehbvm.com/Article/details/gevbtlmyz.sHtML

[S50] C++：格式化数字
来源：http://www.share.fehbvm.com/Article/details/gemvrvbaa.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fehbvm.com/Article/details/ggscawmyz.sHtML

[S51] C++：显式类型转换
来源：http://baike.hesvh.cn/Article/details/ggkdqfuka.sHtML

static_cast<double>(a) / b
来源：http://www.share.hesvh.cn/Article/details/gsumxoxqn.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.zdbjq.cn/Article/details/girgjqeiz.sHtML


<!-- 参考信息 -->