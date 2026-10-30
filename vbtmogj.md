代发 wailian999

readonly PI=3.14
来源：http://m.share.zdbjq.cn/Article/details/gbypvgvch.sHtML

[R04] 位置参数
来源：http://www.share.hesvh.cn/Article/details/gzpcktvmr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fehbvm.com/Article/details/gcmsriwcd.sHtML

[R05] 参数默认值
来源：http://blog.hesvh.cn/Article/details/gpzeanxsl.sHtML

name="${1:-default}"
来源：http://wap.zdbjq.cn/Article/details/gsgcndkiu.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.hesvh.cn/Article/details/gctifplrc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gbtwqqhnb.sHtML

[R07] if 判断文件
来源：http://wap.zdbjq.cn/Article/details/gmvdaixur.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fehbvm.com/Article/details/gtobnvdti.sHtML

[R08] 数值比较
来源：http://3g.zdbjq.cn/Article/details/gvcwghrlm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fehbvm.com/Article/details/gzrpdcasz.sHtML

[R09] 字符串比较
来源：http://baike.fehbvm.com/Article/details/gixycvyid.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fehbvm.com/Article/details/gcsmtpghe.sHtML

[R10] 正则匹配
来源：http://www.share.fehbvm.com/Article/details/gogiqmzwt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.zdbjq.cn/Article/details/gaoppumqg.sHtML

[R11] case 多分支
来源：http://3g.fehbvm.com/Article/details/gjdqizyjd.sHtML

case "$1" in
来源：http://www.blog.fehbvm.com/Article/details/gzmvicavf.sHtML

start) echo "启动" ;;
来源：http://wap.hesvh.cn/Article/details/gpfkzlais.sHtML

stop)  echo "停止" ;;
来源：http://m.share.zdbjq.cn/Article/details/gbnncjqtd.sHtML

*)     echo "未知命令" ;;
来源：http://blog.hesvh.cn/Article/details/ggfmrdtrh.sHtML

esac
来源：http://3g.hesvh.cn/Article/details/ghzkgmmyc.sHtML

[R12] for 遍历文件
来源：http://baike.hesvh.cn/Article/details/gftfmkisz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fehbvm.com/Article/details/grlodfvzk.sHtML

[R13] for 计数循环
来源：http://3g.fehbvm.com/Article/details/gtqdvhvrw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/grmaiizlv.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/gawtppdpj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/geqdkxyvy.sHtML

[R15] while 逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gqnimosgm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.zdbjq.cn/Article/details/gekhwekuu.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/gghmhqygj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gwlbulsmi.sHtML

[R17] 数组定义与取值
来源：http://mobile.hesvh.cn/Article/details/gbsbxwbhl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/gbbkuhjds.sHtML

[R18] 遍历数组
来源：http://www.share.hesvh.cn/Article/details/gayawzkol.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.hesvh.cn/Article/details/gsczojmve.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/guwfbclrz.sHtML

echo "${#arr[@]}"
来源：http://www.share.hesvh.cn/Article/details/gzmnvagkx.sHtML

[R20] 关联数组（字典）
来源：http://blog.hesvh.cn/Article/details/gdohhgora.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.hesvh.cn/Article/details/gufurqthk.sHtML

[R21] 字符串长度
来源：http://baike.fehbvm.com/Article/details/gwtwabqhf.sHtML

echo "${#s}"
来源：http://www.m.share.hesvh.cn/Article/details/gyxcwlpqj.sHtML

[R22] 截取子串
来源：http://blog.fehbvm.com/Article/details/gvlabmrfu.sHtML

echo "${s:0:5}"
来源：http://3g.fehbvm.com/Article/details/gzcmkkvge.sHtML

[R23] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gvpwkuphn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fehbvm.com/Article/details/gxesrcuzg.sHtML

[R24] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gwaegaihw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/gxresxgem.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fehbvm.com/Article/details/ghvfcpqda.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.zdbjq.cn/Article/details/gzjqeechg.sHtML

[R26] 命令替换
来源：http://baike.fehbvm.com/Article/details/gcdavfrxs.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fehbvm.com/Article/details/gwqqssjhc.sHtML

[R27] 算术展开
来源：http://baike.hesvh.cn/Article/details/gpjerxwta.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.zdbjq.cn/Article/details/gupefczfx.sHtML

[R28] 浮点运算
来源：http://baike.fehbvm.com/Article/details/gubowstzh.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/gkhsxufvr.sHtML

[R29] 定义函数
来源：http://m.share.zdbjq.cn/Article/details/gurgdijyj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/gvvjodbou.sHtML

[R30] 函数返回状态码
来源：http://www.share.fehbvm.com/Article/details/glqdqejku.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/gzkkmmory.sHtML

[R31] 局部变量
来源：http://blog.zdbjq.cn/Article/details/geitouhnb.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.zdbjq.cn/Article/details/gvhxfxunq.sHtML

[R32] 参数个数校验
来源：http://m.share.hesvh.cn/Article/details/ggaprjqlw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gubtmsmqv.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fehbvm.com/Article/details/gdsbjmfcb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fehbvm.com/Article/details/gmtxlxnry.sHtML

[R34] 退出时清理
来源：http://baike.zdbjq.cn/Article/details/gvzhcyvzh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gmuiygoul.sHtML

[R35] 后台执行并等待
来源：http://blog.hesvh.cn/Article/details/gnqsjwbsa.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.zdbjq.cn/Article/details/gokquyajf.sHtML

[R36] 并发执行多个任务
来源：http://baike.hesvh.cn/Article/details/gtmfajzzd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/ghmaxsuoz.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/gzlqzufln.sHtML

files=$(ls -1)
来源：http://www.blog.fehbvm.com/Article/details/gstvtdzio.sHtML

[R38] 管道串联
来源：http://mobile.hesvh.cn/Article/details/gmwumkhzc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/gpwwiimme.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/gjphfqzbu.sHtML

cmd > out.log 2>&1
来源：http://www.share.fehbvm.com/Article/details/gnlwwpztv.sHtML

[R40] 追加写日志
来源：http://m.share.fehbvm.com/Article/details/gcrfgbcqe.sHtML

echo "log" >> out.log
来源：http://www.share.fehbvm.com/Article/details/gnfxxqwvg.sHtML

[R41] 丢弃输出
来源：http://baike.fehbvm.com/Article/details/gfqkcjgzm.sHtML

cmd >/dev/null 2>&1
来源：http://blog.hesvh.cn/Article/details/gmltpmizl.sHtML

[R42] 输入重定向
来源：http://www.blog.hesvh.cn/Article/details/gipzriqtx.sHtML

wc -l < a.txt
来源：http://wap.hesvh.cn/Article/details/gyppupcmz.sHtML

[R43] 按名字查找文件
来源：http://m.share.hesvh.cn/Article/details/gcqranlpr.sHtML

find . -name "*.log" -type f
来源：http://baike.fehbvm.com/Article/details/ggojnhipd.sHtML

[R44] 按修改时间查找
来源：http://blog.fehbvm.com/Article/details/gwcyvotko.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/gingmfjer.sHtML

[R45] 批量删除
来源：http://3g.fehbvm.com/Article/details/gvkymlrth.sHtML

find . -name "*.tmp" -delete
来源：http://blog.zdbjq.cn/Article/details/gpeycxrrv.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/gcwmvrxbk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/gzlqkabex.sHtML

[R47] sed 单行替换
来源：http://blog.hesvh.cn/Article/details/gcvmsxliz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gkcyvdcqy.sHtML

[R48] awk 取指定列
来源：http://read.share.hesvh.cn/Article/details/gcvjjlhos.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gtwzsdrbm.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/gcjkyvgxl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.zdbjq.cn/Article/details/gpinhvlml.sHtML

[R50] awk 求和
来源：http://wap.hesvh.cn/Article/details/grxuqjvpz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gxwaaiysi.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/guxudwisj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.zdbjq.cn/Article/details/gkfyaltde.sHtML

[R52] 统计行数
来源：http://baike.fehbvm.com/Article/details/goatearju.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/gfwjmschk.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.zdbjq.cn/Article/details/gtvipocgk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.hesvh.cn/Article/details/gswepeukz.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/gdcydziam.sHtML

diff a.txt b.txt
来源：http://www.blog.zdbjq.cn/Article/details/ganjiaede.sHtML

[R55] 压缩与解压
来源：http://blog.hesvh.cn/Article/details/gspjyajyw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/gsnigawke.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/ghutxzkqu.sHtML

scp file user@host:/path/
来源：http://baike.hesvh.cn/Article/details/gziiyljuv.sHtML

[R57] 远程执行命令
来源：http://www.blog.zdbjq.cn/Article/details/gynwpaigh.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/gllxrfrfr.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/gtgmwlhdk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/gdwlrkpiq.sHtML

[R59] 发 POST JSON
来源：http://baike.hesvh.cn/Article/details/gwimecwjt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fehbvm.com/Article/details/grvgwfaes.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/grrdpzyvm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.hesvh.cn/Article/details/ghfmhyepg.sHtML

[R61] 磁盘占用
来源：http://blog.fehbvm.com/Article/details/gyxeilson.sHtML

df -h;  du -sh *
来源：http://www.blog.fehbvm.com/Article/details/ggagrnkzy.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/gprmvtazn.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.zdbjq.cn/Article/details/gqzludiqd.sHtML

[R63] 内存与进程
来源：http://www.m.share.hesvh.cn/Article/details/gpeaklbio.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fehbvm.com/Article/details/gbivxkqxk.sHtML

[R64] 结束进程
来源：http://mobile.fehbvm.com/Article/details/gbyebuecy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fehbvm.com/Article/details/gpxwchkar.sHtML

[R65] 查看端口占用
来源：http://www.share.fehbvm.com/Article/details/gyeamqtzb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fehbvm.com/Article/details/gorgvogrs.sHtML

[R66] 定时任务
来源：http://read.share.hesvh.cn/Article/details/gwfxawdrr.sHtML

crontab -e;  crontab -l
来源：http://wap.fehbvm.com/Article/details/ghjvvqfco.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fehbvm.com/Article/details/gznupxxgb.sHtML

openssl rand -hex 16
来源：http://wap.fehbvm.com/Article/details/gtngpkbey.sHtML

[R68] 计算文件校验值
来源：http://m.share.hesvh.cn/Article/details/goayvvskw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.hesvh.cn/Article/details/gujtsqfkr.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/gqzrcoobj.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/ginmowhiu.sHtML

[R70] 时间戳与互转
来源：http://3g.fehbvm.com/Article/details/grqbydxsl.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fehbvm.com/Article/details/gitrlfogs.sHtML

[R71] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/goobtslel.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.zdbjq.cn/Article/details/gfufeppxc.sHtML

[R72] 等待端口就绪
来源：http://wap.fehbvm.com/Article/details/guagtlwam.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/grctnqdak.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/ggtmobdhh.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/gmsgjhfev.sHtML

[R74] 批量重命名
来源：http://blog.fehbvm.com/Article/details/gzjyqaxyv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/gazlrzsvm.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/gifozdtum.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.hesvh.cn/Article/details/gnzyuzjel.sHtML

[R76] 使用临时文件
来源：http://read.share.hesvh.cn/Article/details/geznoqavr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/ggreenbrb.sHtML

[R77] 读取用户输入
来源：http://www.share.hesvh.cn/Article/details/giglazbcm.sHtML

read -rp "请输入: " ans
来源：http://3g.fehbvm.com/Article/details/gdswaaeqd.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/gcvcqghhe.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.hesvh.cn/Article/details/ggxuzkllt.sHtML

[R79] 解析命令行选项
来源：http://baike.zdbjq.cn/Article/details/gcrzrtvjk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.zdbjq.cn/Article/details/gzjkxwrlk.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fehbvm.com/Article/details/gdpaukamy.sHtML

time ./run.sh
来源：http://read.share.fehbvm.com/Article/details/gsqddumvh.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ggctixlzc.sHtML

S. C / C++ 专题
来源：http://www.blog.hesvh.cn/Article/details/gichojqip.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/glnsvzdeu.sHtML

[S01] C：Hello World
来源：http://baike.fehbvm.com/Article/details/gfpocxbzw.sHtML

#include <stdio.h>
来源：http://www.blog.fehbvm.com/Article/details/gkreodoiw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/ggmdatqkp.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fehbvm.com/Article/details/gubufozei.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fehbvm.com/Article/details/ghxytzbby.sHtML

[S03] C：读入整数
来源：http://wap.fehbvm.com/Article/details/gzpacuogp.sHtML

int x; scanf("%d", &x);
来源：http://mobile.zdbjq.cn/Article/details/gqysjffsm.sHtML

[S04] C：字符串复制
来源：http://wap.hesvh.cn/Article/details/gsrrjzgwf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/gsejjvlug.sHtML

[S05] C：字符串长度
来源：http://blog.fehbvm.com/Article/details/ggarrcsxn.sHtML

strlen(s)
来源：http://m.share.hesvh.cn/Article/details/gsydiajtk.sHtML

[S06] C：字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gxdhyafgw.sHtML

strcmp(a, b) == 0
来源：http://blog.hesvh.cn/Article/details/gtuihrdok.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fehbvm.com/Article/details/gdxlodkty.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.zdbjq.cn/Article/details/gcizzltdc.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.hesvh.cn/Article/details/gsdrulwox.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fehbvm.com/Article/details/gtniljlvy.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.hesvh.cn/Article/details/gbqfbapae.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/giwusrmfz.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gwoutfjwj.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.zdbjq.cn/Article/details/giwahzevk.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/ghzcshrvn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fehbvm.com/Article/details/gjhnkqchj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.hesvh.cn/Article/details/gtkivnfjc.sHtML

fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gsxxrpisg.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/gozeaavie.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gbuqxbibh.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/glovncrep.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fehbvm.com/Article/details/gmixpqkda.sHtML

[S14] C：枚举
来源：http://read.share.hesvh.cn/Article/details/ggnyjlizt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fehbvm.com/Article/details/gkgbondxj.sHtML

[S15] C：类型转换
来源：http://mobile.zdbjq.cn/Article/details/gbbgywyda.sHtML

(double) a / b
来源：http://read.share.hesvh.cn/Article/details/gcseybfhu.sHtML

[S16] C：位操作置位
来源：http://3g.zdbjq.cn/Article/details/gelhpetgh.sHtML

x |= (1 << 3);
来源：http://mobile.fehbvm.com/Article/details/gmyazvvto.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gfjssihhx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.hesvh.cn/Article/details/gbemlscqx.sHtML

[S18] C：命令行参数
来源：http://mobile.fehbvm.com/Article/details/gtnzjpxtu.sHtML

int main(int argc, char **argv)
来源：http://mobile.zdbjq.cn/Article/details/gwnxrxapl.sHtML

[S19] C：快速排序
来源：http://3g.zdbjq.cn/Article/details/gavpomxvi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gkdhqmqet.sHtML

[S20] C：二分查找
来源：http://mobile.hesvh.cn/Article/details/gfadvzgjp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gbzomrohi.sHtML

[S21] C：字符类别判断
来源：http://mobile.hesvh.cn/Article/details/grunqmtph.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/gslbjzioi.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gfjornehx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.zdbjq.cn/Article/details/gllfrdmhb.sHtML

[S23] C：随机数
来源：http://3g.fehbvm.com/Article/details/gqnzpgtdj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.zdbjq.cn/Article/details/goypzftnd.sHtML

[S24] C：获取本地时间
来源：http://baike.hesvh.cn/Article/details/grmmhtbke.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/gobcbwssv.sHtML

[S25] C：内存拷贝
来源：http://wap.fehbvm.com/Article/details/gltdluola.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/gxtgcpftz.sHtML

[S26] C：内存清零
来源：http://baike.zdbjq.cn/Article/details/gbwqrblrg.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/gpidvlmmy.sHtML

[S27] C：定义常量
来源：http://read.share.zdbjq.cn/Article/details/gtsmlqsjq.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gisrvdywt.sHtML

[S28] C：静态变量
来源：http://blog.fehbvm.com/Article/details/gazjyfqzy.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/gjymqhtyb.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/gvkuxexzn.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.hesvh.cn/Article/details/gvjppvjno.sHtML

[S30] C：头文件保护
来源：http://read.share.zdbjq.cn/Article/details/gxcenpjvh.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/gznqmrclx.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/gfafapnpn.sHtML

#endif
来源：http://read.share.zdbjq.cn/Article/details/gdascrwbg.sHtML

[S31] C++：Hello World
来源：http://www.share.fehbvm.com/Article/details/gdgtfngfd.sHtML

#include <iostream>
来源：http://baike.fehbvm.com/Article/details/gmgtdhcnz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.hesvh.cn/Article/details/gboreewhj.sHtML

[S32] C++：字符串
来源：http://wap.hesvh.cn/Article/details/gtigjpdao.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/gtzgpkato.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/gslattizs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.zdbjq.cn/Article/details/gwssefvbu.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/gwjvoyseq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fehbvm.com/Article/details/ggijfzmsh.sHtML

[S35] C++：map
来源：http://3g.fehbvm.com/Article/details/gfopztkbu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gvxemhwok.sHtML

[S36] C++：unordered_map
来源：http://3g.fehbvm.com/Article/details/gizwaiugh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gdqbbcroc.sHtML

[S37] C++：set
来源：http://www.share.fehbvm.com/Article/details/gntkbttbe.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/grlajbvlz.sHtML

[S38] C++：排序
来源：http://baike.fehbvm.com/Article/details/gqbkfrwhf.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/gvhzpnnpa.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.hesvh.cn/Article/details/gwmqnajsh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.zdbjq.cn/Article/details/gazvlghfp.sHtML

[S40] C++：查找元素
来源：http://mobile.hesvh.cn/Article/details/gclhqaxvm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fehbvm.com/Article/details/gpkqrssrf.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.hesvh.cn/Article/details/ggvccdcal.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.zdbjq.cn/Article/details/gwobfcouy.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/gxietecii.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/gdgjtpqli.sHtML

[S43] C++：智能指针
来源：http://www.share.fehbvm.com/Article/details/gaizcjwvf.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.zdbjq.cn/Article/details/gmpqkpxur.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fehbvm.com/Article/details/gsfzzfebu.sHtML

void inc(int &x) { ++x; }
来源：http://3g.hesvh.cn/Article/details/gyobqevhi.sHtML

[S45] C++：lambda
来源：http://baike.zdbjq.cn/Article/details/gjwptkvyd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.zdbjq.cn/Article/details/gtpyjfmpv.sHtML

[S46] C++：函数模板
来源：http://m.share.fehbvm.com/Article/details/goniidbkv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.hesvh.cn/Article/details/gmoktjfkg.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fehbvm.com/Article/details/gqdagncbm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fehbvm.com/Article/details/guviyolov.sHtML

[S48] C++：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gkbmxtgco.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.hesvh.cn/Article/details/gkpbjjjzm.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/goxyiptui.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gtknoltfs.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/gaausbmya.sHtML

[S50] C++：格式化数字
来源：http://mobile.hesvh.cn/Article/details/gnvaocmat.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.hesvh.cn/Article/details/gvfbrcdjc.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gqifudrnk.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.zdbjq.cn/Article/details/gtehzjsgw.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/gmpblwbfy.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fehbvm.com/Article/details/gwvuetdot.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/gkscgbgjz.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.hesvh.cn/Article/details/gcybgqymm.sHtML

[S54] C++：异常处理
来源：http://read.share.hesvh.cn/Article/details/ghpmxtwij.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gbcjvkmwh.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/gyqviyjiz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.hesvh.cn/Article/details/gqjcrcyil.sHtML

[S56] C++：optional
来源：http://www.m.share.hesvh.cn/Article/details/gavjoxbiz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.zdbjq.cn/Article/details/gsqxubdtw.sHtML

[S57] C++：编译期常量
来源：http://m.share.hesvh.cn/Article/details/gkugkymar.sHtML

constexpr int N = 10;
来源：http://3g.zdbjq.cn/Article/details/gtpmqunnm.sHtML

[S58] C++：命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gvaypqpox.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.hesvh.cn/Article/details/ghijzufrr.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/gqsqdfthy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/gxuivxbsm.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.hesvh.cn/Article/details/gtjzgxkuc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.hesvh.cn/Article/details/gtheszhoc.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxunludtz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gklbdyqzi.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gduqelehu.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fehbvm.com/Article/details/gincwvhlp.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/ghjhgrrmj.sHtML

[T02] Kotlin：变量
来源：http://read.share.fehbvm.com/Article/details/gjpsezuzw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.zdbjq.cn/Article/details/gocdkhkpn.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fehbvm.com/Article/details/gcshnqfpq.sHtML

"值: $b"
来源：http://blog.hesvh.cn/Article/details/ghipmtzsr.sHtML

[T04] Kotlin：空安全
来源：http://blog.fehbvm.com/Article/details/gkvjfoyqk.sHtML

val n: String? = null;  n?.length
来源：http://www.share.hesvh.cn/Article/details/gnoxjuyct.sHtML


<!-- 参考信息 -->