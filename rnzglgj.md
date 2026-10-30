代发 wailian999

set -euo pipefail
来源：http://mobile.zdbjq.cn/Article/details/gizmlvlkl.sHtML

[R02] 变量赋值与使用
来源：http://read.share.hesvh.cn/Article/details/gldcnmlwy.sHtML

name="Tom"; echo "$name"
来源：http://wap.hesvh.cn/Article/details/gxbersvjl.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/glwatvsmb.sHtML

readonly PI=3.14
来源：http://www.blog.zdbjq.cn/Article/details/gtfvmzjlv.sHtML

[R04] 位置参数
来源：http://www.share.fehbvm.com/Article/details/gtkmujkji.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/ghjfcwkip.sHtML

[R05] 参数默认值
来源：http://www.share.fehbvm.com/Article/details/gshuinwsv.sHtML

name="${1:-default}"
来源：http://3g.hesvh.cn/Article/details/gqwifneeo.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gieqlbuqm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gzlgjcfqg.sHtML

[R07] if 判断文件
来源：http://www.m.share.zdbjq.cn/Article/details/gryttapkg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/gonkkxnvl.sHtML

[R08] 数值比较
来源：http://mobile.hesvh.cn/Article/details/gxtntzgyv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fehbvm.com/Article/details/gsifwszzj.sHtML

[R09] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/gmszgnzfz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gjfevzsek.sHtML

[R10] 正则匹配
来源：http://3g.zdbjq.cn/Article/details/grdtjlifc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gwbvxcuha.sHtML

[R11] case 多分支
来源：http://wap.hesvh.cn/Article/details/gtypkfwsq.sHtML

case "$1" in
来源：http://3g.zdbjq.cn/Article/details/gbkezcqhd.sHtML

start) echo "启动" ;;
来源：http://m.share.zdbjq.cn/Article/details/gkgbzujrg.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/gjaxwhrds.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.zdbjq.cn/Article/details/gipeyvcxt.sHtML

esac
来源：http://mobile.hesvh.cn/Article/details/gtzithyrx.sHtML

[R12] for 遍历文件
来源：http://wap.fehbvm.com/Article/details/gbvuhdctj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.zdbjq.cn/Article/details/gehyjhxke.sHtML

[R13] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/gjwrodudi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gnnenpwnd.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/gyelwzrmh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/ghljmsvvu.sHtML

[R15] while 逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gipjeusrz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fehbvm.com/Article/details/gcgqkslpy.sHtML

[R16] until 等待条件
来源：http://baike.fehbvm.com/Article/details/gjuqpbjxv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gdamufzna.sHtML

[R17] 数组定义与取值
来源：http://www.share.fehbvm.com/Article/details/gloxdyywd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.zdbjq.cn/Article/details/govauhkfw.sHtML

[R18] 遍历数组
来源：http://www.share.hesvh.cn/Article/details/gourvvjqq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fehbvm.com/Article/details/ghvbtwczz.sHtML

[R19] 数组长度
来源：http://3g.zdbjq.cn/Article/details/ginbzzija.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fehbvm.com/Article/details/gvrytvucd.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.hesvh.cn/Article/details/gmbuntckb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/gaupknzfm.sHtML

[R21] 字符串长度
来源：http://wap.zdbjq.cn/Article/details/gjqwyzbsb.sHtML

echo "${#s}"
来源：http://3g.fehbvm.com/Article/details/gutlqgwvy.sHtML

[R22] 截取子串
来源：http://blog.fehbvm.com/Article/details/gwkborpux.sHtML

echo "${s:0:5}"
来源：http://m.share.fehbvm.com/Article/details/gnqbmgmgu.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gscckhgib.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.hesvh.cn/Article/details/gkvccteek.sHtML

[R24] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gffzeyxod.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.zdbjq.cn/Article/details/gzmzovpal.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fehbvm.com/Article/details/gliukqmwy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/gqicclosi.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/ghsejnqvi.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/gikbhnebc.sHtML

[R27] 算术展开
来源：http://www.share.fehbvm.com/Article/details/gajfsigmh.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/gwiudadpt.sHtML

[R28] 浮点运算
来源：http://wap.zdbjq.cn/Article/details/gvdvdajna.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.hesvh.cn/Article/details/gdkplsmle.sHtML

[R29] 定义函数
来源：http://www.share.fehbvm.com/Article/details/gdrwxdirg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/gpztvoyxr.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/gjdbsbwni.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/gwxgsjbsp.sHtML

[R31] 局部变量
来源：http://read.share.zdbjq.cn/Article/details/gldqerbkn.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.zdbjq.cn/Article/details/gyjqlkfgx.sHtML

[R32] 参数个数校验
来源：http://mobile.hesvh.cn/Article/details/ghwzyksbe.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjbdjlbfm.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/ggfyyaqmq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.zdbjq.cn/Article/details/gpknihxtu.sHtML

[R34] 退出时清理
来源：http://m.share.fehbvm.com/Article/details/glbrqfvne.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gryqtyofy.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/geavwcgmm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fehbvm.com/Article/details/giyihekyd.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fehbvm.com/Article/details/guedtusen.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/gzgtsmoyg.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.hesvh.cn/Article/details/ghokexuxn.sHtML

files=$(ls -1)
来源：http://baike.hesvh.cn/Article/details/ggpitsuos.sHtML

[R38] 管道串联
来源：http://blog.fehbvm.com/Article/details/gorcqovib.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.hesvh.cn/Article/details/gbjzhckoc.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fehbvm.com/Article/details/gufhtpaey.sHtML

cmd > out.log 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gvnmhfftn.sHtML

[R40] 追加写日志
来源：http://m.share.zdbjq.cn/Article/details/gsnwzoprl.sHtML

echo "log" >> out.log
来源：http://www.share.zdbjq.cn/Article/details/gkimvhpmu.sHtML

[R41] 丢弃输出
来源：http://read.share.hesvh.cn/Article/details/gudpbafuz.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fehbvm.com/Article/details/gtoyojugk.sHtML

[R42] 输入重定向
来源：http://www.share.zdbjq.cn/Article/details/gxxclkqhk.sHtML

wc -l < a.txt
来源：http://baike.fehbvm.com/Article/details/gcfrkbwku.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/gcnmkbmrf.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/gcuislual.sHtML

[R44] 按修改时间查找
来源：http://www.share.zdbjq.cn/Article/details/gowcwmzka.sHtML

find . -mtime -7 -type f
来源：http://wap.hesvh.cn/Article/details/gkmbncavt.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/glgpsglyl.sHtML

find . -name "*.tmp" -delete
来源：http://baike.zdbjq.cn/Article/details/gmwnmhgme.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/gnlletqga.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.zdbjq.cn/Article/details/gmleybhgq.sHtML

[R47] sed 单行替换
来源：http://mobile.fehbvm.com/Article/details/gmflqnvmz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fehbvm.com/Article/details/glxknptjs.sHtML

[R48] awk 取指定列
来源：http://www.blog.hesvh.cn/Article/details/ghypfjntm.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gsjfceivz.sHtML

[R49] awk 带条件
来源：http://www.share.hesvh.cn/Article/details/gggwvggvb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.hesvh.cn/Article/details/gipszosso.sHtML

[R50] awk 求和
来源：http://read.share.hesvh.cn/Article/details/gqqxjxluh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/grbnuiwcq.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fehbvm.com/Article/details/gprrzkmrx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.zdbjq.cn/Article/details/gmplcbhro.sHtML

[R52] 统计行数
来源：http://wap.hesvh.cn/Article/details/gbxjsnwte.sHtML

wc -l a.txt
来源：http://wap.fehbvm.com/Article/details/gvmsubsvy.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fehbvm.com/Article/details/gmeqjhjqm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.hesvh.cn/Article/details/ghrqeltxf.sHtML

[R54] 比较两个文件
来源：http://wap.zdbjq.cn/Article/details/gckusapmz.sHtML

diff a.txt b.txt
来源：http://read.share.hesvh.cn/Article/details/goqvojhly.sHtML

[R55] 压缩与解压
来源：http://read.share.zdbjq.cn/Article/details/gcslkxbge.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/gmseooxhf.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gguzcyanj.sHtML

scp file user@host:/path/
来源：http://3g.fehbvm.com/Article/details/gvcognrui.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fehbvm.com/Article/details/gcvckxdfa.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/gjhulmsqg.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/gdsnwwnzx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/gwxavprlz.sHtML

[R59] 发 POST JSON
来源：http://baike.fehbvm.com/Article/details/gnekxqewq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.hesvh.cn/Article/details/ghltwdfxt.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/getpxacif.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/ggjjppcmc.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/gmnwtsepj.sHtML

df -h;  du -sh *
来源：http://3g.fehbvm.com/Article/details/gwbwnttsw.sHtML

[R62] 找最占空间的文件
来源：http://m.share.hesvh.cn/Article/details/gyuzwzrlq.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/gwykmwzpw.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/gqkucodsg.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.zdbjq.cn/Article/details/gekwvmreq.sHtML

[R64] 结束进程
来源：http://blog.hesvh.cn/Article/details/gvofvsnyi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/gauajkhfz.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gwfwbjvzb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.zdbjq.cn/Article/details/gjryvcduq.sHtML

[R66] 定时任务
来源：http://mobile.zdbjq.cn/Article/details/ggxelhfvn.sHtML

crontab -e;  crontab -l
来源：http://baike.hesvh.cn/Article/details/gxzfalofa.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.zdbjq.cn/Article/details/gvcizfhpd.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/gajgnvabr.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fehbvm.com/Article/details/gwfvdiphd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fehbvm.com/Article/details/gfwrghwjg.sHtML

[R69] 生成随机密码
来源：http://www.share.zdbjq.cn/Article/details/gpuftdcch.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.hesvh.cn/Article/details/galpubivk.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/glzcidbqs.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.zdbjq.cn/Article/details/gifhojnnn.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/grxunyngy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fehbvm.com/Article/details/ggfcwkwum.sHtML

[R72] 等待端口就绪
来源：http://www.blog.hesvh.cn/Article/details/gpcvrgecz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gcnqvhnha.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/ggjtawwtq.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/gjscgfojd.sHtML

[R74] 批量重命名
来源：http://read.share.fehbvm.com/Article/details/gzzslmzne.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fehbvm.com/Article/details/gchbzugnz.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gcmgwfwpz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.zdbjq.cn/Article/details/gkmaqtfkx.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/gujyjmwyb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gvvdlzyxq.sHtML

[R77] 读取用户输入
来源：http://3g.zdbjq.cn/Article/details/gpkyggjma.sHtML

read -rp "请输入: " ans
来源：http://blog.zdbjq.cn/Article/details/gzpzeowpu.sHtML

[R78] 交互式菜单
来源：http://www.m.share.zdbjq.cn/Article/details/gwxqqwqlf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.zdbjq.cn/Article/details/geybwcufr.sHtML

[R79] 解析命令行选项
来源：http://www.share.fehbvm.com/Article/details/gvwegvclf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.zdbjq.cn/Article/details/gdzrqnjef.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/giwkhfynl.sHtML

time ./run.sh
来源：http://baike.fehbvm.com/Article/details/grnwcpqec.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzmzyggiy.sHtML

S. C / C++ 专题
来源：http://3g.zdbjq.cn/Article/details/giwnkcawt.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gowhwwjbf.sHtML

[S01] C：Hello World
来源：http://3g.zdbjq.cn/Article/details/gwnstzzqd.sHtML

#include <stdio.h>
来源：http://www.share.hesvh.cn/Article/details/ghfowhzyc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/gwmsyctwt.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/gcbotbhtl.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fehbvm.com/Article/details/gqpadbnxh.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gpevkbrtm.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.zdbjq.cn/Article/details/gbcbabmlc.sHtML

[S04] C：字符串复制
来源：http://www.m.share.zdbjq.cn/Article/details/geirpzksr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gydpndcqq.sHtML

[S05] C：字符串长度
来源：http://m.share.zdbjq.cn/Article/details/glnkqbzqf.sHtML

strlen(s)
来源：http://m.share.zdbjq.cn/Article/details/gxapwecgj.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/ggznqkqte.sHtML

strcmp(a, b) == 0
来源：http://baike.hesvh.cn/Article/details/gbpwuszrr.sHtML

[S07] C：数组遍历求和
来源：http://baike.zdbjq.cn/Article/details/gslnddqji.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.hesvh.cn/Article/details/glntxoxdv.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.zdbjq.cn/Article/details/guhvlgzdc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/gfoumnzmo.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fehbvm.com/Article/details/gvqugwelz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/glqaubtlf.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.zdbjq.cn/Article/details/gbveqogjq.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.zdbjq.cn/Article/details/grzegfhuh.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gqxxgyrar.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fehbvm.com/Article/details/guadgkpen.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gwjazhwlj.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/gudalzbxn.sHtML

[S12] C：写文件
来源：http://wap.zdbjq.cn/Article/details/gthxmecjf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/guiadhxpj.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/ggpfywrfx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.hesvh.cn/Article/details/geitrfatv.sHtML

[S14] C：枚举
来源：http://mobile.hesvh.cn/Article/details/gxabjcbyp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.zdbjq.cn/Article/details/gblgjucgz.sHtML

[S15] C：类型转换
来源：http://blog.fehbvm.com/Article/details/gtyfjjnid.sHtML

(double) a / b
来源：http://mobile.zdbjq.cn/Article/details/gebfrhujr.sHtML

[S16] C：位操作置位
来源：http://baike.zdbjq.cn/Article/details/geatosmnd.sHtML

x |= (1 << 3);
来源：http://3g.fehbvm.com/Article/details/grtgfspgt.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gdojeytjq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fehbvm.com/Article/details/gmidemdhi.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/gnzopsyjz.sHtML

int main(int argc, char **argv)
来源：http://mobile.zdbjq.cn/Article/details/gghbflqlf.sHtML

[S19] C：快速排序
来源：http://read.share.hesvh.cn/Article/details/gkhuklbsk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/geutgiwwn.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/gzgeppaoz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gnusoufqi.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/gmahmbhhl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fehbvm.com/Article/details/gvuglpvfz.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/geirycmfk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.zdbjq.cn/Article/details/gikhhjstz.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/gzcenbimx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/gfhthsntg.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/gjhkdsuaf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/gttosicav.sHtML

[S25] C：内存拷贝
来源：http://baike.hesvh.cn/Article/details/guzfxgjpa.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.hesvh.cn/Article/details/gymcuypet.sHtML

[S26] C：内存清零
来源：http://www.share.hesvh.cn/Article/details/gnxoylqah.sHtML

memset(a, 0, sizeof a);
来源：http://3g.hesvh.cn/Article/details/gpahkwxyz.sHtML

[S27] C：定义常量
来源：http://baike.zdbjq.cn/Article/details/ghjymogqh.sHtML

const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gewzflgne.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/gntugdyph.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gaelisaap.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/gjkgxpgdb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.zdbjq.cn/Article/details/gvmwkwkvx.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/guiegfree.sHtML

#ifndef X_H
来源：http://www.blog.hesvh.cn/Article/details/gadcayrpu.sHtML

#define X_H
来源：http://read.share.fehbvm.com/Article/details/gsgngdbtu.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/gokorsttx.sHtML

[S31] C++：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/ghfuasfvp.sHtML

#include <iostream>
来源：http://www.blog.zdbjq.cn/Article/details/gflzbpxyo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/gsjbrisiu.sHtML

[S32] C++：字符串
来源：http://www.blog.zdbjq.cn/Article/details/ghshabqfz.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.zdbjq.cn/Article/details/gnqdsfgaa.sHtML

[S33] C++：vector 增删
来源：http://blog.zdbjq.cn/Article/details/gdgccocqi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/glnnmvizp.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fehbvm.com/Article/details/gquvaglyb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.zdbjq.cn/Article/details/guomevfem.sHtML

[S35] C++：map
来源：http://3g.hesvh.cn/Article/details/gptuzkntq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gqrhoqqxm.sHtML

[S36] C++：unordered_map
来源：http://read.share.zdbjq.cn/Article/details/gsusnzrxu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gwbxjmxpm.sHtML

[S37] C++：set
来源：http://www.blog.hesvh.cn/Article/details/gtckbxqna.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.zdbjq.cn/Article/details/gsxqtjfcr.sHtML

[S38] C++：排序
来源：http://www.m.share.hesvh.cn/Article/details/gtkjncvld.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gqtncsbvh.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.zdbjq.cn/Article/details/ghknuxewn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.zdbjq.cn/Article/details/gnbsmtjki.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/gvmpnwqoq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.zdbjq.cn/Article/details/gkxqowvsi.sHtML

[S41] C++：类与构造函数
来源：http://blog.fehbvm.com/Article/details/geywjahxi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/gedwolyxy.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.hesvh.cn/Article/details/goxpvprlm.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fehbvm.com/Article/details/gecrleddv.sHtML

[S43] C++：智能指针
来源：http://www.share.fehbvm.com/Article/details/gftqmdusa.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.zdbjq.cn/Article/details/glgkzlunq.sHtML

[S44] C++：引用传参
来源：http://baike.fehbvm.com/Article/details/gnnfrihkk.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.zdbjq.cn/Article/details/gbigvunvj.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/gyvoufbaa.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fehbvm.com/Article/details/gaqgjbjjs.sHtML

[S46] C++：函数模板
来源：http://wap.fehbvm.com/Article/details/gsozornll.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.hesvh.cn/Article/details/gktgyuydj.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.hesvh.cn/Article/details/gfclxofff.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gklfzqqmz.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gjbaatvfv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/gplqbpohm.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.hesvh.cn/Article/details/ggjlmcwbx.sHtML

[S49] C++：写文件
来源：http://mobile.fehbvm.com/Article/details/gimmjgpwr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.hesvh.cn/Article/details/gxutjwxhs.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.zdbjq.cn/Article/details/goxvuvhnq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/gvstctjbh.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fehbvm.com/Article/details/gyauinlej.sHtML

static_cast<double>(a) / b
来源：http://3g.fehbvm.com/Article/details/gfiezfkak.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/gmgaxmfdu.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.hesvh.cn/Article/details/gutgpmzbi.sHtML

[S53] C++：移动语义
来源：http://www.share.zdbjq.cn/Article/details/gopgrsbyb.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.zdbjq.cn/Article/details/gilkzdscy.sHtML

[S54] C++：异常处理
来源：http://blog.zdbjq.cn/Article/details/ggebgcvxh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fehbvm.com/Article/details/gjhkcjuci.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fehbvm.com/Article/details/gmhjqueef.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/gdfmzuhnk.sHtML

[S56] C++：optional
来源：http://www.share.hesvh.cn/Article/details/glcayafdx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/gzhiwszpm.sHtML

[S57] C++：编译期常量
来源：http://mobile.zdbjq.cn/Article/details/ghularfve.sHtML

constexpr int N = 10;
来源：http://baike.hesvh.cn/Article/details/gryyqlesy.sHtML

[S58] C++：命名空间
来源：http://m.share.hesvh.cn/Article/details/gjolefxxz.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/ggupbpggp.sHtML

[S59] C++：静态断言
来源：http://m.share.fehbvm.com/Article/details/gpxgoigfk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.zdbjq.cn/Article/details/glxwrorll.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.hesvh.cn/Article/details/geuylbbwc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fehbvm.com/Article/details/guhdaenwb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gquhmdtuu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/gwpqavyco.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gluaeukmh.sHtML

[T01] Kotlin：Hello World
来源：http://baike.zdbjq.cn/Article/details/gbfvehlac.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/ggjnwqdnf.sHtML

[T02] Kotlin：变量
来源：http://www.share.hesvh.cn/Article/details/ghueqcedh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.hesvh.cn/Article/details/gywdlpdeq.sHtML


<!-- 参考信息 -->