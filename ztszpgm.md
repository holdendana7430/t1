代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://blog.hesvh.cn/Article/details/gorrusdbn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fehbvm.com/Article/details/gtrbsuegu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.zdbjq.cn/Article/details/gnofnlufj.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fehbvm.com/Article/details/gamwjnbnb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gegmlglol.sHtML

[Q90] 生成序号列
来源：http://www.share.zdbjq.cn/Article/details/ghkqntzpz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.zdbjq.cn/Article/details/gsauswwto.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzyfinwfd.sHtML

R. Bash 专题
来源：http://mobile.zdbjq.cn/Article/details/gcefrqzxq.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxxshjfud.sHtML

[R01] shebang 与严格模式
来源：http://blog.fehbvm.com/Article/details/gylfbtzyj.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fehbvm.com/Article/details/gxmlqrket.sHtML

set -euo pipefail
来源：http://mobile.hesvh.cn/Article/details/gljstglwg.sHtML

[R02] 变量赋值与使用
来源：http://blog.hesvh.cn/Article/details/ginjucqcb.sHtML

name="Tom"; echo "$name"
来源：http://read.share.zdbjq.cn/Article/details/gnuypbllh.sHtML

[R03] 只读变量
来源：http://www.blog.hesvh.cn/Article/details/gegvgdnjw.sHtML

readonly PI=3.14
来源：http://www.blog.fehbvm.com/Article/details/gxwqijwar.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/gqmclvenr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.zdbjq.cn/Article/details/gadlrrthy.sHtML

[R05] 参数默认值
来源：http://www.share.fehbvm.com/Article/details/gcmpoksxb.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/gcxacxotp.sHtML

[R06] 判断命令是否存在
来源：http://m.share.hesvh.cn/Article/details/gngeiqjde.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbveduilf.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/gchipavvg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.zdbjq.cn/Article/details/gudagssdf.sHtML

[R08] 数值比较
来源：http://www.blog.fehbvm.com/Article/details/gtodwugxd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.hesvh.cn/Article/details/gxpywfypv.sHtML

[R09] 字符串比较
来源：http://wap.fehbvm.com/Article/details/gmrnddgnr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.zdbjq.cn/Article/details/gdfmweyzp.sHtML

[R10] 正则匹配
来源：http://baike.fehbvm.com/Article/details/gzrqkihxn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fehbvm.com/Article/details/gzxweijzy.sHtML

[R11] case 多分支
来源：http://blog.hesvh.cn/Article/details/gjdfcroua.sHtML

case "$1" in
来源：http://www.blog.hesvh.cn/Article/details/gtffescdk.sHtML

start) echo "启动" ;;
来源：http://wap.zdbjq.cn/Article/details/gddousjzt.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.hesvh.cn/Article/details/gibasgqqn.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.hesvh.cn/Article/details/gcjdcczie.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/gilnykqiu.sHtML

[R12] for 遍历文件
来源：http://m.share.fehbvm.com/Article/details/gpxwtojuy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.zdbjq.cn/Article/details/geuhvjnie.sHtML

[R13] for 计数循环
来源：http://www.blog.hesvh.cn/Article/details/gqlooonnj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gwvlrpmpr.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/geipyhlud.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/guylgwshe.sHtML

[R15] while 逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gznnlzniw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.hesvh.cn/Article/details/gqvxsrvlh.sHtML

[R16] until 等待条件
来源：http://baike.fehbvm.com/Article/details/gsevdhxij.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gkkowqrhh.sHtML

[R17] 数组定义与取值
来源：http://blog.zdbjq.cn/Article/details/gyxxpokjh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.hesvh.cn/Article/details/guboywimx.sHtML

[R18] 遍历数组
来源：http://mobile.zdbjq.cn/Article/details/gpysbhjnw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fehbvm.com/Article/details/gvosbaznp.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gdveqmejw.sHtML

echo "${#arr[@]}"
来源：http://baike.hesvh.cn/Article/details/gminjrscu.sHtML

[R20] 关联数组（字典）
来源：http://read.share.hesvh.cn/Article/details/genpvqesf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.hesvh.cn/Article/details/gbnrajpfr.sHtML

[R21] 字符串长度
来源：http://3g.hesvh.cn/Article/details/gzxchhmki.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/gxvcloxna.sHtML

[R22] 截取子串
来源：http://m.share.hesvh.cn/Article/details/goqceudco.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/gjrgtqtjn.sHtML

[R23] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/ghnkfawbs.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.hesvh.cn/Article/details/gvjmoctdn.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gpbxnhvmh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.hesvh.cn/Article/details/gnykyjuwa.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.zdbjq.cn/Article/details/ghjupnvnv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fehbvm.com/Article/details/gcbemgoll.sHtML

[R26] 命令替换
来源：http://baike.fehbvm.com/Article/details/gqtmrjdvx.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.zdbjq.cn/Article/details/giddghzbf.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/gsvrpprfm.sHtML

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/gtqmnbywr.sHtML

[R28] 浮点运算
来源：http://m.share.hesvh.cn/Article/details/gwnkmlbod.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.hesvh.cn/Article/details/gsawthqxn.sHtML

[R29] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gsbtuhbuf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/gszmvwsqo.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/gokzeaask.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/gkvillkyq.sHtML

[R31] 局部变量
来源：http://m.share.zdbjq.cn/Article/details/gbvvapogj.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fehbvm.com/Article/details/ggfwigxqj.sHtML

[R32] 参数个数校验
来源：http://baike.zdbjq.cn/Article/details/gvekkprlv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gvqcjiqgo.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fehbvm.com/Article/details/gafmwdwdl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.hesvh.cn/Article/details/gwqtdjsaq.sHtML

[R34] 退出时清理
来源：http://www.share.zdbjq.cn/Article/details/gpyndnvbs.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gmsppsuaf.sHtML

[R35] 后台执行并等待
来源：http://www.share.hesvh.cn/Article/details/gvdensmkf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.zdbjq.cn/Article/details/gdmhcqzem.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/gitorxznx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fehbvm.com/Article/details/gzgbhjwxu.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fehbvm.com/Article/details/gslqhpzli.sHtML

files=$(ls -1)
来源：http://wap.hesvh.cn/Article/details/ggkauptfa.sHtML

[R38] 管道串联
来源：http://wap.fehbvm.com/Article/details/gnshrujno.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fehbvm.com/Article/details/gobpwfhbs.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.hesvh.cn/Article/details/gvjpzvaul.sHtML

cmd > out.log 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gusvulicj.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/gaubqatpt.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/gzljcetwf.sHtML

[R41] 丢弃输出
来源：http://wap.zdbjq.cn/Article/details/glpkebnjs.sHtML

cmd >/dev/null 2>&1
来源：http://wap.hesvh.cn/Article/details/gtnejgzfe.sHtML

[R42] 输入重定向
来源：http://read.share.hesvh.cn/Article/details/gvqswzzdz.sHtML

wc -l < a.txt
来源：http://blog.fehbvm.com/Article/details/gigbvrjwd.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/gzawkszww.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/gsncnykaz.sHtML

[R44] 按修改时间查找
来源：http://blog.fehbvm.com/Article/details/gdgmbyncq.sHtML

find . -mtime -7 -type f
来源：http://baike.zdbjq.cn/Article/details/gmgdghuli.sHtML

[R45] 批量删除
来源：http://3g.hesvh.cn/Article/details/gnxcujktc.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/gfbnffdtg.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/ghysvbavh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gkbtoqvzk.sHtML

[R47] sed 单行替换
来源：http://www.m.share.zdbjq.cn/Article/details/gitasjeer.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fehbvm.com/Article/details/gfcmarofc.sHtML

[R48] awk 取指定列
来源：http://www.share.fehbvm.com/Article/details/gdwcjzdgr.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.hesvh.cn/Article/details/guvobjnwf.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/glszssmrt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fehbvm.com/Article/details/goftmqcgp.sHtML

[R50] awk 求和
来源：http://m.share.hesvh.cn/Article/details/gwfbhftqc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gdbtxvfxy.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fehbvm.com/Article/details/gdgohzqev.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.zdbjq.cn/Article/details/glfcslihl.sHtML

[R52] 统计行数
来源：http://baike.fehbvm.com/Article/details/gbfvowgyt.sHtML

wc -l a.txt
来源：http://www.share.zdbjq.cn/Article/details/gvnaxovsd.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/goacjeabx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.hesvh.cn/Article/details/ggyiqyqkw.sHtML

[R54] 比较两个文件
来源：http://blog.hesvh.cn/Article/details/gglndhvhq.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/gfiejqmdz.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fehbvm.com/Article/details/gtkhbijew.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.zdbjq.cn/Article/details/gysubayoc.sHtML

[R56] 远程拷贝
来源：http://www.blog.fehbvm.com/Article/details/gamjgumzt.sHtML

scp file user@host:/path/
来源：http://mobile.fehbvm.com/Article/details/gfvsdsmhp.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/gdoryhfva.sHtML

ssh user@host 'uptime'
来源：http://baike.zdbjq.cn/Article/details/ggqcvwhuv.sHtML

[R58] 下载文件
来源：http://mobile.zdbjq.cn/Article/details/guhmkpcna.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.zdbjq.cn/Article/details/gahrsumcy.sHtML

[R59] 发 POST JSON
来源：http://baike.fehbvm.com/Article/details/grafbldzf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/ginlxtswc.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gzlzmxdft.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/guxwibuzb.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/gimxatwla.sHtML

df -h;  du -sh *
来源：http://baike.fehbvm.com/Article/details/gvqjjhllv.sHtML

[R62] 找最占空间的文件
来源：http://3g.hesvh.cn/Article/details/gdklvyiqn.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fehbvm.com/Article/details/gfkagyvtx.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/gxyfimnxo.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.zdbjq.cn/Article/details/gzqrymcyx.sHtML

[R64] 结束进程
来源：http://blog.hesvh.cn/Article/details/gufdayhvy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fehbvm.com/Article/details/gtgholuuj.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/gfhrjlkyh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.zdbjq.cn/Article/details/guojdddcb.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/gkjtsiqyl.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/gvwpdsbkb.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fehbvm.com/Article/details/glncmyqqk.sHtML

openssl rand -hex 16
来源：http://www.blog.hesvh.cn/Article/details/gdliedngq.sHtML

[R68] 计算文件校验值
来源：http://blog.hesvh.cn/Article/details/gwykhvocq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/gvgwlmibn.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/gearwafdc.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.zdbjq.cn/Article/details/gxslxnusc.sHtML

[R70] 时间戳与互转
来源：http://3g.fehbvm.com/Article/details/gdsjreyzt.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fehbvm.com/Article/details/grcolbirg.sHtML

[R71] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gdyiowyml.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/gkkffcjeq.sHtML

[R72] 等待端口就绪
来源：http://read.share.fehbvm.com/Article/details/gijxggyds.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/grutforgg.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/gjtshebkt.sHtML

split -l 1000 big.log part_
来源：http://3g.fehbvm.com/Article/details/gqyawolie.sHtML

[R74] 批量重命名
来源：http://www.m.share.hesvh.cn/Article/details/gldrcxvju.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gthhcbzjl.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/gwzvzmsgm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/gnpbuuiyq.sHtML

[R76] 使用临时文件
来源：http://blog.fehbvm.com/Article/details/gcmqihjio.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gsjmduzry.sHtML

[R77] 读取用户输入
来源：http://www.share.fehbvm.com/Article/details/giyfvsdrv.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/gkrhlbxkj.sHtML

[R78] 交互式菜单
来源：http://wap.hesvh.cn/Article/details/gwhwebdnv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.hesvh.cn/Article/details/gcnsswdav.sHtML

[R79] 解析命令行选项
来源：http://blog.fehbvm.com/Article/details/gmfphhqgx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/gcdmcjikz.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.zdbjq.cn/Article/details/gesarwbyr.sHtML

time ./run.sh
来源：http://3g.zdbjq.cn/Article/details/gynkfbuvk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdfhysotj.sHtML

S. C / C++ 专题
来源：http://baike.zdbjq.cn/Article/details/gwsoejhsh.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gynpytlin.sHtML

[S01] C：Hello World
来源：http://www.share.hesvh.cn/Article/details/gpkcsdoaw.sHtML

#include <stdio.h>
来源：http://blog.fehbvm.com/Article/details/gmohkmyvo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fehbvm.com/Article/details/gzyarjnfu.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/ghjwlvcrv.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.hesvh.cn/Article/details/gzhhiktam.sHtML

[S03] C：读入整数
来源：http://www.blog.fehbvm.com/Article/details/grgvyiljn.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fehbvm.com/Article/details/gzrtltcji.sHtML

[S04] C：字符串复制
来源：http://wap.hesvh.cn/Article/details/gpfddgduv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.zdbjq.cn/Article/details/gsespsbxk.sHtML

[S05] C：字符串长度
来源：http://mobile.fehbvm.com/Article/details/gplsqxizh.sHtML

strlen(s)
来源：http://m.share.zdbjq.cn/Article/details/gjiovuwde.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/gvmxixwrg.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fehbvm.com/Article/details/gevjouyyb.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/gindxmgas.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/gswfhtyqw.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.hesvh.cn/Article/details/gwacodizs.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.hesvh.cn/Article/details/glnfyzakb.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/gfxejofqy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.hesvh.cn/Article/details/gntbqlnlc.sHtML

[S10] C：指针与解引用
来源：http://www.blog.hesvh.cn/Article/details/gcjrwpuha.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.zdbjq.cn/Article/details/gwlmvtndr.sHtML

[S11] C：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gfoqwyrul.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.hesvh.cn/Article/details/gzgnidutq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/gjsezxseu.sHtML

fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gttawjdlj.sHtML

[S12] C：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gmdabvdym.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gcecfegbo.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/gihwaaqwb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/gmihqglzy.sHtML

[S14] C：枚举
来源：http://3g.hesvh.cn/Article/details/gpuqbvkfi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/gzvqnqudk.sHtML

[S15] C：类型转换
来源：http://blog.zdbjq.cn/Article/details/gnsxhtcma.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/ghpcnykkg.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/goijiojkb.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/gfimqxxxp.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/grlclwvfm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fehbvm.com/Article/details/gfctmtjdy.sHtML

[S18] C：命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gdxbxjvev.sHtML

int main(int argc, char **argv)
来源：http://baike.zdbjq.cn/Article/details/gglbwbpbt.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/gfikkpznb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gbbvsdayk.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/gojvcqxal.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gjymhfzjx.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/gfgesqhxo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.zdbjq.cn/Article/details/gtdcluwhz.sHtML

[S22] C：字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/gdywinpyz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fehbvm.com/Article/details/gwsjraoaf.sHtML

[S23] C：随机数
来源：http://blog.zdbjq.cn/Article/details/ghuszunfh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.hesvh.cn/Article/details/ggsqseffp.sHtML

[S24] C：获取本地时间
来源：http://blog.fehbvm.com/Article/details/glkekikdx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/gzabupvhk.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/glemlhsnk.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.hesvh.cn/Article/details/gbrwowhlk.sHtML

[S26] C：内存清零
来源：http://3g.hesvh.cn/Article/details/gtlqwvxie.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/gyyxzhjfc.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/grjracbvb.sHtML

const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/ghucwtcat.sHtML

[S28] C：静态变量
来源：http://3g.hesvh.cn/Article/details/gydasxqyu.sHtML

static int counter = 0;
来源：http://www.share.hesvh.cn/Article/details/gbzgbtaqh.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/gzjiwbaax.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.hesvh.cn/Article/details/gffidmvoy.sHtML

[S30] C：头文件保护
来源：http://m.share.zdbjq.cn/Article/details/gxcppvmfj.sHtML

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/gnozjovjd.sHtML

#define X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gvkbzzvwe.sHtML

#endif
来源：http://www.m.share.hesvh.cn/Article/details/gmepkkvcv.sHtML

[S31] C++：Hello World
来源：http://www.share.fehbvm.com/Article/details/gnmwlcnmf.sHtML

#include <iostream>
来源：http://mobile.fehbvm.com/Article/details/gowsenmic.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/gmghvxzez.sHtML

[S32] C++：字符串
来源：http://m.share.fehbvm.com/Article/details/ghopvxzln.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.hesvh.cn/Article/details/gidkainpe.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.hesvh.cn/Article/details/gkjtipabz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/gdldxjkof.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/ggfhicuyv.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.zdbjq.cn/Article/details/grofehfcf.sHtML

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/gxbhyydfy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gnniyurzh.sHtML

[S36] C++：unordered_map
来源：http://3g.fehbvm.com/Article/details/gydymermk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gyigacjip.sHtML

[S37] C++：set
来源：http://www.m.share.fehbvm.com/Article/details/gkcgbppjz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.zdbjq.cn/Article/details/gdgoerozw.sHtML

[S38] C++：排序
来源：http://www.m.share.hesvh.cn/Article/details/ggwhvfzil.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gcgykoozb.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/gbbtocnsa.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.zdbjq.cn/Article/details/gmkviwzfl.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/ggdpluxsg.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.zdbjq.cn/Article/details/gqunukufb.sHtML

[S41] C++：类与构造函数
来源：http://3g.zdbjq.cn/Article/details/gnxpqzspe.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/gjdowoikf.sHtML

[S42] C++：继承与虚函数
来源：http://blog.hesvh.cn/Article/details/glxbzbntx.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.hesvh.cn/Article/details/gjvmvfeea.sHtML

[S43] C++：智能指针
来源：http://wap.zdbjq.cn/Article/details/gadbcvgps.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.zdbjq.cn/Article/details/gqjldjmpz.sHtML

[S44] C++：引用传参
来源：http://3g.hesvh.cn/Article/details/gjbyxccje.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/gthnrntac.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/gsedhhwjl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.hesvh.cn/Article/details/gswgoavuf.sHtML

[S46] C++：函数模板
来源：http://baike.zdbjq.cn/Article/details/gvwufotef.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.zdbjq.cn/Article/details/gbhogelkg.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/grzmncvrz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/gsybfkdlw.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gxmaklyzq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.zdbjq.cn/Article/details/gfeaeqpzm.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/gecydplmh.sHtML

[S49] C++：写文件
来源：http://www.blog.fehbvm.com/Article/details/gdltjeocg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.hesvh.cn/Article/details/gtqkdeert.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/gzrwseoyh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fehbvm.com/Article/details/gugwdftii.sHtML

[S51] C++：显式类型转换
来源：http://blog.fehbvm.com/Article/details/gbgotqger.sHtML

static_cast<double>(a) / b
来源：http://3g.hesvh.cn/Article/details/gplqhbcyk.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.zdbjq.cn/Article/details/gsgjhsyzs.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/giynvjhwy.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/ggtccxtlj.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.zdbjq.cn/Article/details/gtyfvsmhp.sHtML

[S54] C++：异常处理
来源：http://blog.fehbvm.com/Article/details/gxlznlheq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/gfaendzgq.sHtML

[S55] C++：结构化绑定
来源：http://3g.hesvh.cn/Article/details/gdldhinpw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.hesvh.cn/Article/details/gmasdbelw.sHtML

[S56] C++：optional
来源：http://3g.zdbjq.cn/Article/details/gynbnqqvw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/gjcqmexch.sHtML

[S57] C++：编译期常量
来源：http://www.blog.hesvh.cn/Article/details/gqhzfinzo.sHtML

constexpr int N = 10;
来源：http://wap.fehbvm.com/Article/details/gufmfovgi.sHtML

[S58] C++：命名空间
来源：http://www.share.zdbjq.cn/Article/details/ggszdqpja.sHtML


<!-- 参考信息 -->