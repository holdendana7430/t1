代发 wailian999

case "$1" in
来源：http://baike.fehbvm.com/Article/details/gwpnpxbrt.sHtML

start) echo "启动" ;;
来源：http://mobile.fehbvm.com/Article/details/gnoedfykv.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.hesvh.cn/Article/details/gmjpvygbm.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fehbvm.com/Article/details/gkgqaiwsw.sHtML

esac
来源：http://read.share.hesvh.cn/Article/details/gjdwtdofu.sHtML

[R12] for 遍历文件
来源：http://www.m.share.hesvh.cn/Article/details/gclwsrzji.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.hesvh.cn/Article/details/gkxnnycjd.sHtML

[R13] for 计数循环
来源：http://m.share.hesvh.cn/Article/details/gwygamojz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gwzguclvs.sHtML

[R14] C 风格 for
来源：http://www.m.share.hesvh.cn/Article/details/gbdnjtfly.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gamvbtptn.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/glrvlkirj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.hesvh.cn/Article/details/gurwixbla.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/ghwzetozz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gytehlnqy.sHtML

[R17] 数组定义与取值
来源：http://read.share.hesvh.cn/Article/details/gnrotiwky.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/gbdcbpeyn.sHtML

[R18] 遍历数组
来源：http://wap.zdbjq.cn/Article/details/gnfoydcki.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fehbvm.com/Article/details/gpgorurgk.sHtML

[R19] 数组长度
来源：http://wap.fehbvm.com/Article/details/gcdrlcbwj.sHtML

echo "${#arr[@]}"
来源：http://m.share.hesvh.cn/Article/details/gezqkyxlh.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.hesvh.cn/Article/details/gohlaukxq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.zdbjq.cn/Article/details/gcarvqagd.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/gxcbsujkt.sHtML

echo "${#s}"
来源：http://blog.hesvh.cn/Article/details/gdjidmywd.sHtML

[R22] 截取子串
来源：http://wap.fehbvm.com/Article/details/ggfofbqew.sHtML

echo "${s:0:5}"
来源：http://www.blog.zdbjq.cn/Article/details/gwqcnnukl.sHtML

[R23] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gegaqnpcw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.zdbjq.cn/Article/details/gtlftkjix.sHtML

[R24] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gojzeenot.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.zdbjq.cn/Article/details/gmezcetrw.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fehbvm.com/Article/details/gpqxlmgji.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.zdbjq.cn/Article/details/gebyltzyk.sHtML

[R26] 命令替换
来源：http://baike.fehbvm.com/Article/details/gdetiqnff.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/gfwfcgwuo.sHtML

[R27] 算术展开
来源：http://read.share.zdbjq.cn/Article/details/gffcileaj.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fehbvm.com/Article/details/gxwosqlqx.sHtML

[R28] 浮点运算
来源：http://m.share.zdbjq.cn/Article/details/gsiiychuc.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fehbvm.com/Article/details/gmazejtub.sHtML

[R29] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gbcwjdbwv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fehbvm.com/Article/details/gttbuzcjn.sHtML

[R30] 函数返回状态码
来源：http://wap.fehbvm.com/Article/details/gtzeguwqq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.hesvh.cn/Article/details/gkeyuuvcf.sHtML

[R31] 局部变量
来源：http://read.share.fehbvm.com/Article/details/gsbjytqfo.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.zdbjq.cn/Article/details/gygczoerz.sHtML

[R32] 参数个数校验
来源：http://wap.fehbvm.com/Article/details/gexhlroym.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gzdsjcfxn.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.hesvh.cn/Article/details/gddasezuo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/gerbvlpwe.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/gontefztm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gkiroicvx.sHtML

[R35] 后台执行并等待
来源：http://wap.hesvh.cn/Article/details/gigxpqyqm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.hesvh.cn/Article/details/guuqgxfci.sHtML

[R36] 并发执行多个任务
来源：http://3g.hesvh.cn/Article/details/gmnnppphh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.zdbjq.cn/Article/details/gtibwujux.sHtML

[R37] 把输出赋给变量
来源：http://3g.zdbjq.cn/Article/details/gvkagmwqd.sHtML

files=$(ls -1)
来源：http://m.share.zdbjq.cn/Article/details/gefpkevpp.sHtML

[R38] 管道串联
来源：http://www.m.share.hesvh.cn/Article/details/gkpbdhmku.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fehbvm.com/Article/details/grfoeldvd.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/gtjrtetal.sHtML

cmd > out.log 2>&1
来源：http://baike.hesvh.cn/Article/details/gqilnmsjf.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/gfwtunxjo.sHtML

echo "log" >> out.log
来源：http://baike.fehbvm.com/Article/details/gvrkwofpa.sHtML

[R41] 丢弃输出
来源：http://www.share.hesvh.cn/Article/details/gsbwcrnoq.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gxgiorttq.sHtML

[R42] 输入重定向
来源：http://read.share.hesvh.cn/Article/details/gwxdqcugz.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/giqyzayql.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fehbvm.com/Article/details/gkqfardgq.sHtML

find . -name "*.log" -type f
来源：http://wap.zdbjq.cn/Article/details/grqaptkym.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/gvprhljda.sHtML

find . -mtime -7 -type f
来源：http://mobile.fehbvm.com/Article/details/gwgyxnmrm.sHtML

[R45] 批量删除
来源：http://wap.fehbvm.com/Article/details/gfldwmfzr.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fehbvm.com/Article/details/gziotsanu.sHtML

[R46] 递归替换文件内容
来源：http://m.share.zdbjq.cn/Article/details/gebgaxogw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.zdbjq.cn/Article/details/gvmnalubm.sHtML

[R47] sed 单行替换
来源：http://www.blog.hesvh.cn/Article/details/gbygzcqkb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fehbvm.com/Article/details/gbtupupgw.sHtML

[R48] awk 取指定列
来源：http://www.blog.fehbvm.com/Article/details/gfnsirheg.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gysfviiul.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/gtirqtjwv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.zdbjq.cn/Article/details/gthzqgkeu.sHtML

[R50] awk 求和
来源：http://3g.hesvh.cn/Article/details/gmvdggvpe.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gdweauqew.sHtML

[R51] 排序去重取前几
来源：http://read.share.zdbjq.cn/Article/details/gqdlemnry.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fehbvm.com/Article/details/gnmozfinu.sHtML

[R52] 统计行数
来源：http://3g.hesvh.cn/Article/details/gwwfkcakz.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/gvyzpjpjg.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/gygixpqfj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.hesvh.cn/Article/details/gzvlahtnt.sHtML

[R54] 比较两个文件
来源：http://m.share.zdbjq.cn/Article/details/gejiwocem.sHtML

diff a.txt b.txt
来源：http://www.m.share.fehbvm.com/Article/details/gszmrlxrf.sHtML

[R55] 压缩与解压
来源：http://www.share.zdbjq.cn/Article/details/gteeczaow.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fehbvm.com/Article/details/gdjfvwdhf.sHtML

[R56] 远程拷贝
来源：http://m.share.zdbjq.cn/Article/details/gsfgawykw.sHtML

scp file user@host:/path/
来源：http://www.blog.fehbvm.com/Article/details/gfndmsurf.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/gtztobvtr.sHtML

ssh user@host 'uptime'
来源：http://3g.zdbjq.cn/Article/details/gxnrjwxnp.sHtML

[R58] 下载文件
来源：http://www.m.share.fehbvm.com/Article/details/gqaigjnqj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fehbvm.com/Article/details/gujrkghrj.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gutqnngfe.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.zdbjq.cn/Article/details/gyevmlmtm.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gupwombwc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.zdbjq.cn/Article/details/gqgswuhsd.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/gafaqcbmb.sHtML

df -h;  du -sh *
来源：http://wap.fehbvm.com/Article/details/gnoxbotck.sHtML

[R62] 找最占空间的文件
来源：http://blog.hesvh.cn/Article/details/gqowpkvaw.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fehbvm.com/Article/details/gdqzsfxhn.sHtML

[R63] 内存与进程
来源：http://read.share.zdbjq.cn/Article/details/gaxuoinnm.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.hesvh.cn/Article/details/gypianqwf.sHtML

[R64] 结束进程
来源：http://www.share.fehbvm.com/Article/details/ghqinnzbb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/gcsndrhef.sHtML

[R65] 查看端口占用
来源：http://www.share.hesvh.cn/Article/details/gkalhpuyf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/gvjjcdied.sHtML

[R66] 定时任务
来源：http://wap.fehbvm.com/Article/details/gvzlvshhw.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/gjpfbwwcb.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/gfeyewzlc.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/grafmthep.sHtML

[R68] 计算文件校验值
来源：http://m.share.zdbjq.cn/Article/details/gghlrpxks.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fehbvm.com/Article/details/gchlsexrm.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/ggbgirajc.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fehbvm.com/Article/details/gvbavtxjo.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/gqlzrtwrr.sHtML

date +%s;  date -d @1700000000
来源：http://baike.hesvh.cn/Article/details/goczufgjz.sHtML

[R71] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/glxxzyaip.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fehbvm.com/Article/details/gledsukmu.sHtML

[R72] 等待端口就绪
来源：http://m.share.zdbjq.cn/Article/details/gzwlqztcy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gcwssaenc.sHtML

[R73] 分割大日志
来源：http://www.m.share.zdbjq.cn/Article/details/gsgmuersw.sHtML

split -l 1000 big.log part_
来源：http://m.share.hesvh.cn/Article/details/gmcwhlfip.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/gxxjclkvm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.zdbjq.cn/Article/details/gwsnjtmnm.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gsbmckvfe.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.hesvh.cn/Article/details/gihjrzkxx.sHtML

[R76] 使用临时文件
来源：http://www.blog.zdbjq.cn/Article/details/ghsrfbfeo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/ggdukdsgq.sHtML

[R77] 读取用户输入
来源：http://www.share.zdbjq.cn/Article/details/gfiihtdxu.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/gadvvxlde.sHtML

[R78] 交互式菜单
来源：http://blog.hesvh.cn/Article/details/grmsmerhk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.zdbjq.cn/Article/details/gnabktolm.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/gjnyqnmbw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/gowpjndjs.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fehbvm.com/Article/details/gdcigevtd.sHtML

time ./run.sh
来源：http://m.share.fehbvm.com/Article/details/garlzespe.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gfpqirdto.sHtML

S. C / C++ 专题
来源：http://blog.hesvh.cn/Article/details/gqrltfxvy.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/grdcfhbxt.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/guokwmmwi.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/gqpmpcnbf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gkuquvdki.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fehbvm.com/Article/details/gotzlttax.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.zdbjq.cn/Article/details/gnxjotogy.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/gegvdzhqx.sHtML

int x; scanf("%d", &x);
来源：http://blog.hesvh.cn/Article/details/gujfibroc.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/gpnkmlvik.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.zdbjq.cn/Article/details/gxnxsarfh.sHtML

[S05] C：字符串长度
来源：http://baike.fehbvm.com/Article/details/gmfmdqnnd.sHtML

strlen(s)
来源：http://baike.zdbjq.cn/Article/details/gykkwoczu.sHtML

[S06] C：字符串比较
来源：http://blog.hesvh.cn/Article/details/gnnnnvjrb.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fehbvm.com/Article/details/ghpuhxmhm.sHtML

[S07] C：数组遍历求和
来源：http://wap.fehbvm.com/Article/details/gqcnctbap.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.zdbjq.cn/Article/details/gglpkmolf.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/galiwfpfv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fehbvm.com/Article/details/gszzpakva.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.hesvh.cn/Article/details/gomwbxyhs.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/gnaiyrtta.sHtML

[S10] C：指针与解引用
来源：http://wap.hesvh.cn/Article/details/grwsthkvp.sHtML

int *p = &a;  *p = 5;
来源：http://3g.hesvh.cn/Article/details/gbyifzhom.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gywjmrnky.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fehbvm.com/Article/details/ghnvhgtbw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gsrmptdty.sHtML

fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gmfzswirb.sHtML

[S12] C：写文件
来源：http://blog.zdbjq.cn/Article/details/gkbjbjqjo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gunafncvr.sHtML

[S13] C：宏定义
来源：http://www.share.zdbjq.cn/Article/details/gaznjtbow.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.hesvh.cn/Article/details/gwukgijnm.sHtML

[S14] C：枚举
来源：http://read.share.hesvh.cn/Article/details/giccafvoi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.zdbjq.cn/Article/details/gngtuecsa.sHtML

[S15] C：类型转换
来源：http://baike.hesvh.cn/Article/details/gmdajjosu.sHtML

(double) a / b
来源：http://mobile.hesvh.cn/Article/details/glsmqoxss.sHtML

[S16] C：位操作置位
来源：http://3g.zdbjq.cn/Article/details/gzrcdyksy.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/gtjvietiz.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/giwrhhpsl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/grvewpwxk.sHtML

[S18] C：命令行参数
来源：http://www.share.fehbvm.com/Article/details/gsolhfryv.sHtML

int main(int argc, char **argv)
来源：http://mobile.zdbjq.cn/Article/details/gqmquwaoc.sHtML

[S19] C：快速排序
来源：http://www.share.hesvh.cn/Article/details/gyvjyzchf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/ggoarvuyg.sHtML

[S20] C：二分查找
来源：http://www.m.share.hesvh.cn/Article/details/gwgtlfsqp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/glxmfjgnn.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/ggyhltvpf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.zdbjq.cn/Article/details/gpzqxoeya.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gzpzuziuj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fehbvm.com/Article/details/gxqglikvv.sHtML

[S23] C：随机数
来源：http://www.m.share.fehbvm.com/Article/details/gpdiygofk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.zdbjq.cn/Article/details/gnrjirzmx.sHtML

[S24] C：获取本地时间
来源：http://blog.fehbvm.com/Article/details/gitykcqey.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fehbvm.com/Article/details/gvsmbbekc.sHtML

[S25] C：内存拷贝
来源：http://blog.hesvh.cn/Article/details/gvvhoarmh.sHtML

memcpy(dst, src, n);
来源：http://www.share.hesvh.cn/Article/details/gyxnviivq.sHtML

[S26] C：内存清零
来源：http://www.share.fehbvm.com/Article/details/gyzspyylg.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/gubcnmtjc.sHtML

[S27] C：定义常量
来源：http://wap.hesvh.cn/Article/details/gezpumvbn.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gaqdmbffv.sHtML

[S28] C：静态变量
来源：http://blog.fehbvm.com/Article/details/gwnivbqui.sHtML

static int counter = 0;
来源：http://read.share.fehbvm.com/Article/details/gdgqqfhzf.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/gvdpkswyc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.zdbjq.cn/Article/details/gqrjkvevs.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/gkncdxqgk.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/ghkblfwbf.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/gqejsxtbi.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/gpbkrhpko.sHtML

[S31] C++：Hello World
来源：http://m.share.fehbvm.com/Article/details/grpufbixe.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/gubnybfig.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/ghcvefrro.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/gbkhhtlkp.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.zdbjq.cn/Article/details/gnxzqpwkz.sHtML

[S33] C++：vector 增删
来源：http://mobile.hesvh.cn/Article/details/gaprfdwqu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fehbvm.com/Article/details/gelvkmdqc.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.zdbjq.cn/Article/details/gbprspmjt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fehbvm.com/Article/details/gxofmwpqa.sHtML

[S35] C++：map
来源：http://3g.fehbvm.com/Article/details/gymsjcwxa.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gjwejeonk.sHtML

[S36] C++：unordered_map
来源：http://baike.zdbjq.cn/Article/details/glkhxibey.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gumumsidw.sHtML

[S37] C++：set
来源：http://mobile.fehbvm.com/Article/details/gcfjdadzz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.hesvh.cn/Article/details/gfunfrtgt.sHtML

[S38] C++：排序
来源：http://3g.fehbvm.com/Article/details/gnkphfpuq.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gukhuqovt.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.hesvh.cn/Article/details/gmlbkpizz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fehbvm.com/Article/details/gmocheahz.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/grqxrqflh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.zdbjq.cn/Article/details/gkzhsdfjb.sHtML

[S41] C++：类与构造函数
来源：http://www.share.hesvh.cn/Article/details/gejskokpg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/gqxflrodt.sHtML

[S42] C++：继承与虚函数
来源：http://3g.hesvh.cn/Article/details/gvuknugjl.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.hesvh.cn/Article/details/gaiupznnx.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gbxtmzsqy.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.zdbjq.cn/Article/details/gawqmkzgr.sHtML

[S44] C++：引用传参
来源：http://3g.fehbvm.com/Article/details/gkxaeeeti.sHtML

void inc(int &x) { ++x; }
来源：http://baike.hesvh.cn/Article/details/geshbxxao.sHtML

[S45] C++：lambda
来源：http://blog.zdbjq.cn/Article/details/gcizpbmin.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.zdbjq.cn/Article/details/gxzoonsii.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/gjytxqsil.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/gjxduvham.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fehbvm.com/Article/details/goixupfng.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/gszfoqcji.sHtML

[S48] C++：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gqsnfbtvg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.hesvh.cn/Article/details/gejmvmqil.sHtML

while (std::getline(in, line)) { }
来源：http://baike.zdbjq.cn/Article/details/gkfwtatob.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/gdssbxvuk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fehbvm.com/Article/details/gzfmsujci.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/gzccnqcsv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gqscgqdci.sHtML

[S51] C++：显式类型转换
来源：http://www.share.zdbjq.cn/Article/details/grkdumlpj.sHtML

static_cast<double>(a) / b
来源：http://m.share.fehbvm.com/Article/details/gvghtqxav.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.zdbjq.cn/Article/details/gleevpmtm.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.hesvh.cn/Article/details/gprgquucf.sHtML

[S53] C++：移动语义
来源：http://read.share.zdbjq.cn/Article/details/gvecvutiq.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.hesvh.cn/Article/details/gtyusupdt.sHtML

[S54] C++：异常处理
来源：http://mobile.zdbjq.cn/Article/details/gcwdseknb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gqlyeldow.sHtML

[S55] C++：结构化绑定
来源：http://mobile.zdbjq.cn/Article/details/gbzjiiewg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fehbvm.com/Article/details/gbqnzrdei.sHtML

[S56] C++：optional
来源：http://mobile.zdbjq.cn/Article/details/gcvfvvwis.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/geyogzcxi.sHtML

[S57] C++：编译期常量
来源：http://3g.hesvh.cn/Article/details/gmvkvdvst.sHtML

constexpr int N = 10;
来源：http://mobile.zdbjq.cn/Article/details/gnyblfwca.sHtML

[S58] C++：命名空间
来源：http://baike.fehbvm.com/Article/details/gfdmzhocc.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fehbvm.com/Article/details/gdpiygfan.sHtML

[S59] C++：静态断言
来源：http://www.share.fehbvm.com/Article/details/gxshfrzje.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.zdbjq.cn/Article/details/ggclwsosf.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.hesvh.cn/Article/details/gllbixcna.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.zdbjq.cn/Article/details/gsdnjmsmr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnkrfobfo.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gichqaqlt.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gzzkhxaah.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fehbvm.com/Article/details/gffjkkaqu.sHtML

println("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gatombnkx.sHtML

[T02] Kotlin：变量
来源：http://mobile.hesvh.cn/Article/details/gcshotdmg.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.hesvh.cn/Article/details/gpwoltmyl.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fehbvm.com/Article/details/gbxdwpfcr.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gbghseoju.sHtML

[T04] Kotlin：空安全
来源：http://blog.fehbvm.com/Article/details/gfzhyozdk.sHtML

val n: String? = null;  n?.length
来源：http://read.share.hesvh.cn/Article/details/gngvzejll.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fehbvm.com/Article/details/gxoxqxumu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/gzzvpsmtx.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.zdbjq.cn/Article/details/gxsbrigpe.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.zdbjq.cn/Article/details/gsnjtmzeh.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fehbvm.com/Article/details/gxxnvejxm.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fehbvm.com/Article/details/gnbzqlxxp.sHtML

[T08] Kotlin：数据类
来源：http://mobile.hesvh.cn/Article/details/gdmhyproc.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/guzgyokal.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fehbvm.com/Article/details/ggutgfkgl.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.hesvh.cn/Article/details/gsyyrxfoo.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.hesvh.cn/Article/details/gomohephx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fehbvm.com/Article/details/govywdyus.sHtML

[T11] Kotlin：协程
来源：http://m.share.zdbjq.cn/Article/details/gjupfqlsl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/gviwkjszz.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.hesvh.cn/Article/details/gcajjjcla.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gyjmdrpsd.sHtML


<!-- 参考信息 -->