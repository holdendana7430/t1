代发 wailian999

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/gajmwfhmg.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/ghqgwstke.sHtML

[Q85] 数值取整
来源：http://www.m.share.fehbvm.com/Article/details/gxfbhylmf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fehbvm.com/Article/details/gntnqzmgl.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.hesvh.cn/Article/details/gyziqrypk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fehbvm.com/Article/details/ggcmifijb.sHtML

[Q87] JSON 字段做条件
来源：http://blog.hesvh.cn/Article/details/goijkvvdd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fehbvm.com/Article/details/gindujzth.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fehbvm.com/Article/details/gusqcsbbw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.zdbjq.cn/Article/details/grteidzxu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.hesvh.cn/Article/details/goztbvdyz.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gtzgmmgrc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.zdbjq.cn/Article/details/gvryrihjt.sHtML

[Q90] 生成序号列
来源：http://baike.hesvh.cn/Article/details/gaamxldhj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fehbvm.com/Article/details/gveyiqzoo.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/grwnacubh.sHtML

R. Bash 专题
来源：http://read.share.hesvh.cn/Article/details/ggwpeotyt.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjgemamno.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fehbvm.com/Article/details/gqzwusgan.sHtML

#!/usr/bin/env bash
来源：http://blog.zdbjq.cn/Article/details/gfnvkzggo.sHtML

set -euo pipefail
来源：http://m.share.zdbjq.cn/Article/details/gdluzsetx.sHtML

[R02] 变量赋值与使用
来源：http://baike.hesvh.cn/Article/details/gqngpalcz.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fehbvm.com/Article/details/golkliykm.sHtML

[R03] 只读变量
来源：http://baike.zdbjq.cn/Article/details/gljctryfw.sHtML

readonly PI=3.14
来源：http://www.share.zdbjq.cn/Article/details/gonkiwnpu.sHtML

[R04] 位置参数
来源：http://www.blog.fehbvm.com/Article/details/ggsugkuqp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.zdbjq.cn/Article/details/ggihxptkv.sHtML

[R05] 参数默认值
来源：http://www.blog.zdbjq.cn/Article/details/gyqdjmdhb.sHtML

name="${1:-default}"
来源：http://3g.zdbjq.cn/Article/details/gpefqgqhm.sHtML

[R06] 判断命令是否存在
来源：http://www.share.zdbjq.cn/Article/details/ggsofmvvp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gashlzajz.sHtML

[R07] if 判断文件
来源：http://m.share.hesvh.cn/Article/details/gppqfkbsd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/gswzepqhf.sHtML

[R08] 数值比较
来源：http://m.share.zdbjq.cn/Article/details/gxiiqrkpf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/gddbwlpph.sHtML

[R09] 字符串比较
来源：http://baike.fehbvm.com/Article/details/ghhsawlgr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fehbvm.com/Article/details/grvyuroxz.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/gbpomjgia.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fehbvm.com/Article/details/grbkylkuv.sHtML

[R11] case 多分支
来源：http://mobile.fehbvm.com/Article/details/gjdzhjusn.sHtML

case "$1" in
来源：http://www.blog.zdbjq.cn/Article/details/gbqsdhxiu.sHtML

start) echo "启动" ;;
来源：http://www.share.hesvh.cn/Article/details/gnnjcvjcb.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fehbvm.com/Article/details/gssptcrqm.sHtML

*)     echo "未知命令" ;;
来源：http://3g.hesvh.cn/Article/details/gimjgtoxa.sHtML

esac
来源：http://read.share.zdbjq.cn/Article/details/gxdeewihn.sHtML

[R12] for 遍历文件
来源：http://baike.hesvh.cn/Article/details/gggfuzlav.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/gzbghbzef.sHtML

[R13] for 计数循环
来源：http://blog.hesvh.cn/Article/details/gutffkjpf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gogdtzlfm.sHtML

[R14] C 风格 for
来源：http://3g.hesvh.cn/Article/details/gfgyxkbga.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gzpzpbybl.sHtML

[R15] while 逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gbcqdzczq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fehbvm.com/Article/details/gqqpsdiav.sHtML

[R16] until 等待条件
来源：http://3g.hesvh.cn/Article/details/grzljbjaa.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gvngbiiyk.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.zdbjq.cn/Article/details/gnuqwweko.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.zdbjq.cn/Article/details/gtqyaxson.sHtML

[R18] 遍历数组
来源：http://blog.fehbvm.com/Article/details/grkvzmvzi.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.zdbjq.cn/Article/details/gbmrjgwbv.sHtML

[R19] 数组长度
来源：http://baike.hesvh.cn/Article/details/gxxqwunuf.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fehbvm.com/Article/details/gudctmael.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.hesvh.cn/Article/details/gqirdbour.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.hesvh.cn/Article/details/grlwwxidz.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/gxwprbzzl.sHtML

echo "${#s}"
来源：http://mobile.fehbvm.com/Article/details/guhjwodwl.sHtML

[R22] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gpwxnsbsg.sHtML

echo "${s:0:5}"
来源：http://www.blog.zdbjq.cn/Article/details/gmhkztags.sHtML

[R23] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gumzqqgdz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.hesvh.cn/Article/details/gvzwzmrjo.sHtML

[R24] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gvupkrdne.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/gmfdrjzij.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fehbvm.com/Article/details/gyaanrncw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fehbvm.com/Article/details/gfteodtol.sHtML

[R26] 命令替换
来源：http://www.m.share.hesvh.cn/Article/details/gvtpjnyie.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.zdbjq.cn/Article/details/gxcjpgwid.sHtML

[R27] 算术展开
来源：http://wap.zdbjq.cn/Article/details/goxcvehwj.sHtML

echo $((1 + 2 * 3))
来源：http://3g.hesvh.cn/Article/details/gcacjyvrp.sHtML

[R28] 浮点运算
来源：http://www.share.fehbvm.com/Article/details/gzzxvvpbb.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.hesvh.cn/Article/details/gvfdzwaxe.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/ggpfxrzwo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/gozsfibpa.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gnzmnnlha.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/gdafaecdg.sHtML

[R31] 局部变量
来源：http://www.m.share.fehbvm.com/Article/details/glrygjgiu.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.hesvh.cn/Article/details/gunummade.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/glqxphahq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpgirtcwu.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.zdbjq.cn/Article/details/gpcqznxkh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.zdbjq.cn/Article/details/gmzumzbzx.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/gwkhfhoyo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gelsqbwwv.sHtML

[R35] 后台执行并等待
来源：http://wap.zdbjq.cn/Article/details/glfbcwopw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fehbvm.com/Article/details/gqikdmiir.sHtML

[R36] 并发执行多个任务
来源：http://m.share.hesvh.cn/Article/details/gkiobycut.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fehbvm.com/Article/details/gcqpbuyqw.sHtML

[R37] 把输出赋给变量
来源：http://m.share.hesvh.cn/Article/details/genlicqfg.sHtML

files=$(ls -1)
来源：http://www.m.share.fehbvm.com/Article/details/ggdlzqzwv.sHtML

[R38] 管道串联
来源：http://www.blog.hesvh.cn/Article/details/gtexorbjl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.zdbjq.cn/Article/details/gyfranpoq.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fehbvm.com/Article/details/ggexhuqso.sHtML

cmd > out.log 2>&1
来源：http://m.share.hesvh.cn/Article/details/gmfbjozlb.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/gcopkgwrc.sHtML

echo "log" >> out.log
来源：http://read.share.zdbjq.cn/Article/details/gcfrxbxsx.sHtML

[R41] 丢弃输出
来源：http://baike.fehbvm.com/Article/details/gwlfkakqf.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/ggnvlkwns.sHtML

[R42] 输入重定向
来源：http://www.share.zdbjq.cn/Article/details/gmxxkslko.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/gcesbolux.sHtML

[R43] 按名字查找文件
来源：http://www.blog.hesvh.cn/Article/details/gsccgkkbh.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/gglydgomu.sHtML

[R44] 按修改时间查找
来源：http://www.share.hesvh.cn/Article/details/gxfahastt.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fehbvm.com/Article/details/gomboylwn.sHtML

[R45] 批量删除
来源：http://baike.fehbvm.com/Article/details/gkyldidwl.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/gkbbaiqwi.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fehbvm.com/Article/details/gcudsnobp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.zdbjq.cn/Article/details/gzjrrdhyw.sHtML

[R47] sed 单行替换
来源：http://mobile.zdbjq.cn/Article/details/gabvogsdn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/gfsgkjnhb.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/grzlsgxsz.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fehbvm.com/Article/details/grakrwzjx.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/gbavqtenu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fehbvm.com/Article/details/geenjgpqr.sHtML

[R50] awk 求和
来源：http://m.share.fehbvm.com/Article/details/gdwzcurgn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fehbvm.com/Article/details/ghplxucxd.sHtML

[R51] 排序去重取前几
来源：http://www.blog.hesvh.cn/Article/details/ggjfxwcyt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/gyjqitxnc.sHtML

[R52] 统计行数
来源：http://wap.hesvh.cn/Article/details/gtmlxsjap.sHtML

wc -l a.txt
来源：http://wap.fehbvm.com/Article/details/godkjxyao.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.hesvh.cn/Article/details/gampafyox.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.zdbjq.cn/Article/details/gicgxiyqf.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/ghvjlavfb.sHtML

diff a.txt b.txt
来源：http://mobile.zdbjq.cn/Article/details/gpbjwrxpr.sHtML

[R55] 压缩与解压
来源：http://www.m.share.zdbjq.cn/Article/details/gxwoijenv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/gymiilooe.sHtML

[R56] 远程拷贝
来源：http://blog.zdbjq.cn/Article/details/gswbggqoi.sHtML

scp file user@host:/path/
来源：http://read.share.zdbjq.cn/Article/details/gxsjafogo.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/gxjjplpoc.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/giijolxfm.sHtML

[R58] 下载文件
来源：http://www.share.fehbvm.com/Article/details/gwclcabcp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fehbvm.com/Article/details/gskjssrpd.sHtML

[R59] 发 POST JSON
来源：http://baike.fehbvm.com/Article/details/gkoyxnzhj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/ghxedkfeh.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gafnsdnwu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fehbvm.com/Article/details/gaxdppkpx.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/gkydtbiaw.sHtML

df -h;  du -sh *
来源：http://blog.hesvh.cn/Article/details/gyzfpowms.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fehbvm.com/Article/details/gastqlkdw.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.hesvh.cn/Article/details/gkltdcowx.sHtML

[R63] 内存与进程
来源：http://wap.zdbjq.cn/Article/details/gwyxwhkdz.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fehbvm.com/Article/details/grfohtrql.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/gjudledfr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/gnqmpkewh.sHtML

[R65] 查看端口占用
来源：http://m.share.zdbjq.cn/Article/details/gfhjqnoou.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.hesvh.cn/Article/details/grkdrabac.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/gbgmszvke.sHtML

crontab -e;  crontab -l
来源：http://blog.zdbjq.cn/Article/details/glassysqk.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fehbvm.com/Article/details/gbphsvyuq.sHtML

openssl rand -hex 16
来源：http://blog.fehbvm.com/Article/details/guzywafsz.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/gsvjfgpav.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.hesvh.cn/Article/details/gnrwkyohm.sHtML

[R69] 生成随机密码
来源：http://www.share.zdbjq.cn/Article/details/gyqwqxqzt.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.hesvh.cn/Article/details/gfqewaphc.sHtML

[R70] 时间戳与互转
来源：http://3g.zdbjq.cn/Article/details/gfrlfveyv.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/gxjgenyls.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gwooctlap.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fehbvm.com/Article/details/gkxqnyntw.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/gpsqtgtxt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gaazsntoc.sHtML

[R73] 分割大日志
来源：http://3g.hesvh.cn/Article/details/gbzktplog.sHtML

split -l 1000 big.log part_
来源：http://baike.hesvh.cn/Article/details/gswqafvsb.sHtML

[R74] 批量重命名
来源：http://www.m.share.hesvh.cn/Article/details/gvypzzxjr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/gidcwkkyw.sHtML

[R75] 导出环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/giublpnti.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/gcntfgkmq.sHtML

[R76] 使用临时文件
来源：http://mobile.zdbjq.cn/Article/details/ghnchfhyy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/glgavxiki.sHtML

[R77] 读取用户输入
来源：http://read.share.zdbjq.cn/Article/details/ghladwvvk.sHtML

read -rp "请输入: " ans
来源：http://3g.hesvh.cn/Article/details/gfelgwnye.sHtML

[R78] 交互式菜单
来源：http://wap.hesvh.cn/Article/details/gpqfpmrnx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.hesvh.cn/Article/details/gfbjrescg.sHtML

[R79] 解析命令行选项
来源：http://mobile.hesvh.cn/Article/details/goirxysrx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.hesvh.cn/Article/details/geiasqrfw.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.hesvh.cn/Article/details/gpqrdhtsu.sHtML

time ./run.sh
来源：http://www.share.fehbvm.com/Article/details/gtqemzilo.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkcdrpvhd.sHtML

S. C / C++ 专题
来源：http://blog.hesvh.cn/Article/details/gsiespjyg.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gohcslpmc.sHtML

[S01] C：Hello World
来源：http://baike.zdbjq.cn/Article/details/gngiqstux.sHtML

#include <stdio.h>
来源：http://3g.hesvh.cn/Article/details/gbkauxffo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gtiwlpkji.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/gzxmyutje.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.zdbjq.cn/Article/details/gfnjbpelo.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/glrhztiiq.sHtML

int x; scanf("%d", &x);
来源：http://baike.fehbvm.com/Article/details/gtzglcxbe.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/gqbvbkdwy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gyuoxfyjh.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/gpbmcyfzz.sHtML

strlen(s)
来源：http://mobile.fehbvm.com/Article/details/gksdailzg.sHtML

[S06] C：字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gnweausio.sHtML

strcmp(a, b) == 0
来源：http://m.share.fehbvm.com/Article/details/gyriqitwx.sHtML

[S07] C：数组遍历求和
来源：http://blog.hesvh.cn/Article/details/gwmateljh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/gcnxqyfec.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/goftfgawo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.zdbjq.cn/Article/details/gimslhxhi.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.hesvh.cn/Article/details/gumhklxnu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.hesvh.cn/Article/details/geqxoelyy.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/gmeuuybnw.sHtML

int *p = &a;  *p = 5;
来源：http://wap.zdbjq.cn/Article/details/gajviuxjx.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gmyzvfbto.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/gbuenonee.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.hesvh.cn/Article/details/gadqcvuqz.sHtML

fclose(f);
来源：http://baike.hesvh.cn/Article/details/gnaezltcr.sHtML

[S12] C：写文件
来源：http://mobile.fehbvm.com/Article/details/ghrdpysuw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gmlyuoitd.sHtML

[S13] C：宏定义
来源：http://wap.fehbvm.com/Article/details/gnkcgwxvy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fehbvm.com/Article/details/gwgkyxzbj.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/gxykgzicf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.hesvh.cn/Article/details/gplduepzj.sHtML

[S15] C：类型转换
来源：http://blog.fehbvm.com/Article/details/guasmvbsq.sHtML

(double) a / b
来源：http://baike.zdbjq.cn/Article/details/gxhikuffh.sHtML

[S16] C：位操作置位
来源：http://m.share.zdbjq.cn/Article/details/ggeywpsuo.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/gigrelgxt.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fehbvm.com/Article/details/gragbgdhv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/gsecqotgo.sHtML

[S18] C：命令行参数
来源：http://mobile.hesvh.cn/Article/details/ghaaxczwc.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/gthaognvm.sHtML

[S19] C：快速排序
来源：http://www.m.share.hesvh.cn/Article/details/gduizqfkc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gfjbgbfjg.sHtML

[S20] C：二分查找
来源：http://3g.fehbvm.com/Article/details/gqmoqzrpm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gdhwogitm.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/gxignoidp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.hesvh.cn/Article/details/gfrcgxkgm.sHtML

[S22] C：字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/gxlveoxoa.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fehbvm.com/Article/details/gwmioymnt.sHtML

[S23] C：随机数
来源：http://wap.fehbvm.com/Article/details/gxrrlxjfl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.zdbjq.cn/Article/details/gytayghij.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/gpekinktk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gimupzhdd.sHtML

[S25] C：内存拷贝
来源：http://wap.zdbjq.cn/Article/details/goeffmunm.sHtML

memcpy(dst, src, n);
来源：http://mobile.fehbvm.com/Article/details/gbsjmgeln.sHtML

[S26] C：内存清零
来源：http://www.m.share.fehbvm.com/Article/details/gbiygnxfs.sHtML

memset(a, 0, sizeof a);
来源：http://wap.zdbjq.cn/Article/details/gpfbteejg.sHtML

[S27] C：定义常量
来源：http://www.blog.fehbvm.com/Article/details/geusykacl.sHtML

const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gmgggtixx.sHtML

[S28] C：静态变量
来源：http://mobile.fehbvm.com/Article/details/gqupbcxth.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/gmxdngpmv.sHtML

[S29] C：变参函数
来源：http://www.share.fehbvm.com/Article/details/gnxwchctl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/guvmljlhj.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/gvlwkqise.sHtML

#ifndef X_H
来源：http://3g.fehbvm.com/Article/details/gsqmkqqug.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/grqofupvc.sHtML

#endif
来源：http://www.m.share.hesvh.cn/Article/details/gduyocrpn.sHtML

[S31] C++：Hello World
来源：http://wap.fehbvm.com/Article/details/ggmcavzja.sHtML

#include <iostream>
来源：http://m.share.hesvh.cn/Article/details/ghpseibak.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/gpfcbgcbb.sHtML

[S32] C++：字符串
来源：http://baike.fehbvm.com/Article/details/gadbqejms.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.zdbjq.cn/Article/details/glfqlrjcp.sHtML

[S33] C++：vector 增删
来源：http://read.share.zdbjq.cn/Article/details/gjvxhbqxo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.zdbjq.cn/Article/details/gykcynwiq.sHtML

[S34] C++：遍历 vector
来源：http://blog.zdbjq.cn/Article/details/gflwgltks.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/ggbsypjps.sHtML

[S35] C++：map
来源：http://www.blog.hesvh.cn/Article/details/ghjlqdjor.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gqjhszxfd.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/gfylgafog.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gufrphxoy.sHtML

[S37] C++：set
来源：http://www.m.share.zdbjq.cn/Article/details/gjmrjqebw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/glanvrjef.sHtML

[S38] C++：排序
来源：http://www.blog.hesvh.cn/Article/details/gkqhbrhfl.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/giffryijm.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fehbvm.com/Article/details/gifpdyxfl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/gicmixidu.sHtML

[S40] C++：查找元素
来源：http://www.blog.zdbjq.cn/Article/details/gmksljizl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.zdbjq.cn/Article/details/gprusrgsx.sHtML

[S41] C++：类与构造函数
来源：http://read.share.hesvh.cn/Article/details/glmwnzpvq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/ghbdvmojg.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.zdbjq.cn/Article/details/gbucxslmz.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fehbvm.com/Article/details/guxcwgymo.sHtML

[S43] C++：智能指针
来源：http://mobile.zdbjq.cn/Article/details/guuheivwz.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fehbvm.com/Article/details/gsuznissx.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/grjxtbmis.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.hesvh.cn/Article/details/gzegzfnbv.sHtML

[S45] C++：lambda
来源：http://blog.fehbvm.com/Article/details/guedpaxhm.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.zdbjq.cn/Article/details/gdxyoymjl.sHtML

[S46] C++：函数模板
来源：http://blog.zdbjq.cn/Article/details/gknhabwtc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fehbvm.com/Article/details/gylcmmvot.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gracmxhxt.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fehbvm.com/Article/details/grnwgeubo.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gvmozalab.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.hesvh.cn/Article/details/gomwcsujs.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.hesvh.cn/Article/details/glrhrhjhb.sHtML

[S49] C++：写文件
来源：http://3g.zdbjq.cn/Article/details/gofzyqacr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/gluctmzen.sHtML

[S50] C++：格式化数字
来源：http://mobile.zdbjq.cn/Article/details/gucwzkorr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/grgkqqfhz.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/gfczmbvls.sHtML

static_cast<double>(a) / b
来源：http://wap.fehbvm.com/Article/details/gwzehlvjy.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.hesvh.cn/Article/details/gsfusonmw.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.hesvh.cn/Article/details/gmjviaxwk.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/gtsrbblgq.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.hesvh.cn/Article/details/gimgbvgne.sHtML

[S54] C++：异常处理
来源：http://www.share.hesvh.cn/Article/details/gslsqxmds.sHtML


<!-- 参考信息 -->