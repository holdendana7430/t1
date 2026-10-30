代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fehbvm.com/Article/details/gjclbslln.sHtML

[R08] 数值比较
来源：http://wap.zdbjq.cn/Article/details/gaeuadjvd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.zdbjq.cn/Article/details/geqxqugtj.sHtML

[R09] 字符串比较
来源：http://blog.fehbvm.com/Article/details/gctmszdtv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gjeiknrwf.sHtML

[R10] 正则匹配
来源：http://blog.fehbvm.com/Article/details/gtllvcxqe.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/gwhdopvdv.sHtML

[R11] case 多分支
来源：http://m.share.hesvh.cn/Article/details/gmgtmchsp.sHtML

case "$1" in
来源：http://m.share.zdbjq.cn/Article/details/gruurrwrj.sHtML

start) echo "启动" ;;
来源：http://3g.zdbjq.cn/Article/details/gjwectjxo.sHtML

stop)  echo "停止" ;;
来源：http://baike.fehbvm.com/Article/details/glxdjcwio.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/gqtnmdiok.sHtML

esac
来源：http://m.share.hesvh.cn/Article/details/gnaqbobmf.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/glevdgmae.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fehbvm.com/Article/details/gzexmvnsm.sHtML

[R13] for 计数循环
来源：http://read.share.zdbjq.cn/Article/details/gjgcueovk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gvwookcme.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/giqxfzwpj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gmfbtzkde.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/gqrlswlgb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/gnbambkot.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/gfshpwydi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gunjxrpcf.sHtML

[R17] 数组定义与取值
来源：http://www.share.hesvh.cn/Article/details/gxpgidkxm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.hesvh.cn/Article/details/grtotpnaa.sHtML

[R18] 遍历数组
来源：http://3g.hesvh.cn/Article/details/gvtadlpac.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.hesvh.cn/Article/details/ggyexivps.sHtML

[R19] 数组长度
来源：http://www.share.hesvh.cn/Article/details/ggxaqpcco.sHtML

echo "${#arr[@]}"
来源：http://blog.hesvh.cn/Article/details/gszbpkyhh.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/goljvxgja.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fehbvm.com/Article/details/gdltavcsb.sHtML

[R21] 字符串长度
来源：http://3g.zdbjq.cn/Article/details/gqrkodqlt.sHtML

echo "${#s}"
来源：http://blog.fehbvm.com/Article/details/gjifujhde.sHtML

[R22] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gmvlmpxoi.sHtML

echo "${s:0:5}"
来源：http://baike.zdbjq.cn/Article/details/guspyxcug.sHtML

[R23] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gomlrngrp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/glaydfkiq.sHtML

[R24] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/geoeszhvc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.zdbjq.cn/Article/details/gjbxjfnpc.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.zdbjq.cn/Article/details/gzobjpsok.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fehbvm.com/Article/details/glaschrdo.sHtML

[R26] 命令替换
来源：http://3g.zdbjq.cn/Article/details/geffyyidi.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/geemmsqfn.sHtML

[R27] 算术展开
来源：http://m.share.hesvh.cn/Article/details/gaappdlnj.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.hesvh.cn/Article/details/gqeimrpdc.sHtML

[R28] 浮点运算
来源：http://blog.hesvh.cn/Article/details/gndchydlh.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.hesvh.cn/Article/details/gymfmgwpv.sHtML

[R29] 定义函数
来源：http://3g.fehbvm.com/Article/details/gfuxzwxcg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fehbvm.com/Article/details/gwxoesluq.sHtML

[R30] 函数返回状态码
来源：http://m.share.zdbjq.cn/Article/details/grzdfjbfs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/grjhbxssb.sHtML

[R31] 局部变量
来源：http://blog.fehbvm.com/Article/details/gozzsiepi.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.zdbjq.cn/Article/details/gbkzqhika.sHtML

[R32] 参数个数校验
来源：http://m.share.zdbjq.cn/Article/details/gvpvltyyk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxibkrpky.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fehbvm.com/Article/details/gtmkyzdgv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fehbvm.com/Article/details/gocpneins.sHtML

[R34] 退出时清理
来源：http://www.blog.fehbvm.com/Article/details/gtjkqpqht.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gzjjtnhtn.sHtML

[R35] 后台执行并等待
来源：http://blog.fehbvm.com/Article/details/guobubtgx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fehbvm.com/Article/details/gvnhpjjrm.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fehbvm.com/Article/details/gmksdgqbw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fehbvm.com/Article/details/gwwzdvjtw.sHtML

[R37] 把输出赋给变量
来源：http://m.share.hesvh.cn/Article/details/grlpymwrc.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/gkbtjghmk.sHtML

[R38] 管道串联
来源：http://wap.fehbvm.com/Article/details/gzsraqinr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.zdbjq.cn/Article/details/grtplrgfa.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/gxrjdjiwa.sHtML

cmd > out.log 2>&1
来源：http://3g.hesvh.cn/Article/details/gzlghrbdt.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/ggcnhqncx.sHtML

echo "log" >> out.log
来源：http://read.share.fehbvm.com/Article/details/gzkuflwlb.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/gcbrwrigi.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.hesvh.cn/Article/details/ghvsaqezl.sHtML

[R42] 输入重定向
来源：http://mobile.zdbjq.cn/Article/details/gpihvjhak.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/gqsccpenj.sHtML

[R43] 按名字查找文件
来源：http://blog.zdbjq.cn/Article/details/giideuqmd.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/gwqtadbby.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fehbvm.com/Article/details/gjrjqnxhh.sHtML

find . -mtime -7 -type f
来源：http://read.share.hesvh.cn/Article/details/gyncfowkg.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/gbtsonfbj.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fehbvm.com/Article/details/gtuvzhbbc.sHtML

[R46] 递归替换文件内容
来源：http://www.share.zdbjq.cn/Article/details/gjggtziwf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.zdbjq.cn/Article/details/gftzcrelj.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/gcauyucrz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/gpwwqegrx.sHtML

[R48] awk 取指定列
来源：http://www.share.hesvh.cn/Article/details/gkqnjqday.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gxsefgmub.sHtML

[R49] awk 带条件
来源：http://m.share.fehbvm.com/Article/details/gihphqwqt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.hesvh.cn/Article/details/goyrmzlgp.sHtML

[R50] awk 求和
来源：http://wap.zdbjq.cn/Article/details/gnvspsstk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/glbwingye.sHtML

[R51] 排序去重取前几
来源：http://baike.fehbvm.com/Article/details/gpkiaylvq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.zdbjq.cn/Article/details/gmssrvwpn.sHtML

[R52] 统计行数
来源：http://read.share.fehbvm.com/Article/details/ggbmdlqok.sHtML

wc -l a.txt
来源：http://mobile.zdbjq.cn/Article/details/gfefalznm.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.zdbjq.cn/Article/details/gsofcrjwf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/gwufoifey.sHtML

[R54] 比较两个文件
来源：http://mobile.fehbvm.com/Article/details/glafdxwgr.sHtML

diff a.txt b.txt
来源：http://mobile.zdbjq.cn/Article/details/gosavqhgs.sHtML

[R55] 压缩与解压
来源：http://mobile.hesvh.cn/Article/details/ghvvlsrvn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.zdbjq.cn/Article/details/gwmpwzoei.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/gflvkszul.sHtML

scp file user@host:/path/
来源：http://m.share.zdbjq.cn/Article/details/gvtymdzop.sHtML

[R57] 远程执行命令
来源：http://www.m.share.zdbjq.cn/Article/details/grccovycl.sHtML

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/ghsntlyld.sHtML

[R58] 下载文件
来源：http://read.share.zdbjq.cn/Article/details/gzgwtzunc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.zdbjq.cn/Article/details/gxbbiimbk.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/grtxdrsnu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.hesvh.cn/Article/details/guafnxlxr.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gidsasjsu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/gjrqxhkdh.sHtML

[R61] 磁盘占用
来源：http://wap.hesvh.cn/Article/details/gatxoppdj.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/gtnqxqxnq.sHtML

[R62] 找最占空间的文件
来源：http://www.share.hesvh.cn/Article/details/gplgvosbf.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.zdbjq.cn/Article/details/gcvmxsgwl.sHtML

[R63] 内存与进程
来源：http://www.share.zdbjq.cn/Article/details/gxksqkrkb.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/grlzftjsk.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/gmrqfnlvc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/gbpdtpxpp.sHtML

[R65] 查看端口占用
来源：http://read.share.zdbjq.cn/Article/details/gjdrykcny.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fehbvm.com/Article/details/gyjrvbrsw.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/gxquwyrph.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/gopbbclvm.sHtML

[R67] 生成随机十六进制串
来源：http://wap.hesvh.cn/Article/details/gbsvhuujp.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/gxpsezmmh.sHtML

[R68] 计算文件校验值
来源：http://www.share.zdbjq.cn/Article/details/gigmpbltd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fehbvm.com/Article/details/gqrxrbrge.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/gjckbksjn.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fehbvm.com/Article/details/gbjhlzdcw.sHtML

[R70] 时间戳与互转
来源：http://m.share.hesvh.cn/Article/details/gmwqgozor.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.hesvh.cn/Article/details/gmfaiqxoj.sHtML

[R71] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gwzbfluek.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.zdbjq.cn/Article/details/gehxjenxd.sHtML

[R72] 等待端口就绪
来源：http://3g.fehbvm.com/Article/details/ggcdbmqkb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gqobzoscn.sHtML

[R73] 分割大日志
来源：http://read.share.zdbjq.cn/Article/details/gbfrmjtod.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/goeuprdwr.sHtML

[R74] 批量重命名
来源：http://m.share.zdbjq.cn/Article/details/geqtwixuv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/gzvauacbm.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/gocyaqpta.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.zdbjq.cn/Article/details/gaifemvft.sHtML

[R76] 使用临时文件
来源：http://www.share.hesvh.cn/Article/details/gpeapryzw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gojoclloy.sHtML

[R77] 读取用户输入
来源：http://www.m.share.zdbjq.cn/Article/details/gmtkfnuix.sHtML

read -rp "请输入: " ans
来源：http://3g.zdbjq.cn/Article/details/gbzujuvui.sHtML

[R78] 交互式菜单
来源：http://wap.fehbvm.com/Article/details/gmmjxtygo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.hesvh.cn/Article/details/gubszqjvy.sHtML

[R79] 解析命令行选项
来源：http://read.share.hesvh.cn/Article/details/gfcabgayn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fehbvm.com/Article/details/gygprmdar.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.hesvh.cn/Article/details/gwgmuyeue.sHtML

time ./run.sh
来源：http://www.m.share.zdbjq.cn/Article/details/gasbricpb.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grdrmozzp.sHtML

S. C / C++ 专题
来源：http://3g.zdbjq.cn/Article/details/gtvidkpuq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gprensksl.sHtML

[S01] C：Hello World
来源：http://mobile.fehbvm.com/Article/details/gbyajozzt.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/gjihpiawp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/gzabykvjk.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fehbvm.com/Article/details/glgmvootu.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.zdbjq.cn/Article/details/ggclhmfpy.sHtML

[S03] C：读入整数
来源：http://mobile.hesvh.cn/Article/details/geecllxat.sHtML

int x; scanf("%d", &x);
来源：http://baike.hesvh.cn/Article/details/gnerjupcb.sHtML

[S04] C：字符串复制
来源：http://www.share.zdbjq.cn/Article/details/gnwrqmptu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gtjwtlbdq.sHtML

[S05] C：字符串长度
来源：http://baike.zdbjq.cn/Article/details/gstumecsx.sHtML

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/gwnrhqedd.sHtML

[S06] C：字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gjardklil.sHtML

strcmp(a, b) == 0
来源：http://blog.zdbjq.cn/Article/details/gocfuyhom.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fehbvm.com/Article/details/gsqeufvsc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fehbvm.com/Article/details/gvskcnnlp.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fehbvm.com/Article/details/grrdmmrfv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.hesvh.cn/Article/details/gjswezccy.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fehbvm.com/Article/details/gombemcdb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fehbvm.com/Article/details/gcukhiwoq.sHtML

[S10] C：指针与解引用
来源：http://mobile.fehbvm.com/Article/details/gaiiulngi.sHtML

int *p = &a;  *p = 5;
来源：http://baike.hesvh.cn/Article/details/gutfwfuhp.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gfsdnmygz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/gyjtbxvza.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fehbvm.com/Article/details/gafrpcweq.sHtML

fclose(f);
来源：http://3g.fehbvm.com/Article/details/gywpbfwse.sHtML

[S12] C：写文件
来源：http://www.share.zdbjq.cn/Article/details/gstjanqnv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gianmieoi.sHtML

[S13] C：宏定义
来源：http://mobile.hesvh.cn/Article/details/gqrzkirjn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/gzblupptw.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/gtnieszxn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fehbvm.com/Article/details/gifgxmznf.sHtML

[S15] C：类型转换
来源：http://www.share.fehbvm.com/Article/details/geskmkalc.sHtML

(double) a / b
来源：http://read.share.fehbvm.com/Article/details/gzmuekszn.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/gyqjwfbxx.sHtML

x |= (1 << 3);
来源：http://3g.fehbvm.com/Article/details/gweryhmur.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/ghanhqyap.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.hesvh.cn/Article/details/gofcdqjlm.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gmbjikvfb.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/glsgdyoqo.sHtML

[S19] C：快速排序
来源：http://www.share.fehbvm.com/Article/details/gnqsvuevz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gzssvcruz.sHtML

[S20] C：二分查找
来源：http://www.blog.zdbjq.cn/Article/details/gnzokoonc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gzvihnipa.sHtML

[S21] C：字符类别判断
来源：http://wap.fehbvm.com/Article/details/gknhnvmds.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fehbvm.com/Article/details/gsehpbate.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gicpinodc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.hesvh.cn/Article/details/grpfzseqr.sHtML

[S23] C：随机数
来源：http://www.share.hesvh.cn/Article/details/glrpniinu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fehbvm.com/Article/details/gjnchnopy.sHtML

[S24] C：获取本地时间
来源：http://www.share.hesvh.cn/Article/details/gnvstqcpu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.hesvh.cn/Article/details/gvtpfgsqj.sHtML

[S25] C：内存拷贝
来源：http://m.share.zdbjq.cn/Article/details/gfwumouul.sHtML

memcpy(dst, src, n);
来源：http://read.share.fehbvm.com/Article/details/gdqkarsrf.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/gehzvuivy.sHtML

memset(a, 0, sizeof a);
来源：http://baike.hesvh.cn/Article/details/gdtsuyfiz.sHtML

[S27] C：定义常量
来源：http://blog.fehbvm.com/Article/details/gwvhkeork.sHtML

const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/grsflzfwt.sHtML

[S28] C：静态变量
来源：http://www.blog.zdbjq.cn/Article/details/gfstfzldm.sHtML

static int counter = 0;
来源：http://mobile.zdbjq.cn/Article/details/grhceasxe.sHtML

[S29] C：变参函数
来源：http://m.share.zdbjq.cn/Article/details/grdbxafsh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fehbvm.com/Article/details/gawvkwgyz.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/gmgxbzjwu.sHtML

#ifndef X_H
来源：http://www.m.share.zdbjq.cn/Article/details/ggmhdlcnp.sHtML

#define X_H
来源：http://www.m.share.hesvh.cn/Article/details/givlmnimf.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/gvryoltwb.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/gtcdjlqmb.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/gojvadpkp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fehbvm.com/Article/details/gacnsanau.sHtML

[S32] C++：字符串
来源：http://mobile.hesvh.cn/Article/details/guthwqvnj.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/ghvvhfpkt.sHtML

[S33] C++：vector 增删
来源：http://m.share.hesvh.cn/Article/details/geakcllan.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/gztxtubvk.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fehbvm.com/Article/details/gcgyoaojy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/gmnmnszch.sHtML

[S35] C++：map
来源：http://mobile.hesvh.cn/Article/details/gnnagicvy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gykkwkhca.sHtML

[S36] C++：unordered_map
来源：http://3g.fehbvm.com/Article/details/gqkbzfkwd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/grarhmzbj.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/gancapykx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/grtparbbs.sHtML

[S38] C++：排序
来源：http://baike.fehbvm.com/Article/details/gznkxebvn.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.hesvh.cn/Article/details/godbnqkne.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.hesvh.cn/Article/details/gtnrzsjui.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.hesvh.cn/Article/details/giwgxgagk.sHtML

[S40] C++：查找元素
来源：http://www.m.share.hesvh.cn/Article/details/gngdzudoh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fehbvm.com/Article/details/gxctbxeug.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gwzhlyhei.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fehbvm.com/Article/details/gjeilelzq.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.hesvh.cn/Article/details/gqmghrtxj.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fehbvm.com/Article/details/gduutveff.sHtML

[S43] C++：智能指针
来源：http://m.share.zdbjq.cn/Article/details/gaydcbzyc.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.zdbjq.cn/Article/details/gjfmfkauw.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fehbvm.com/Article/details/gfkwyohjc.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fehbvm.com/Article/details/gauzxclvn.sHtML

[S45] C++：lambda
来源：http://m.share.fehbvm.com/Article/details/gysasgbsv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.hesvh.cn/Article/details/golugdwkw.sHtML

[S46] C++：函数模板
来源：http://www.share.fehbvm.com/Article/details/ggcxrcfhi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.zdbjq.cn/Article/details/gvfudutzn.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fehbvm.com/Article/details/gdtiegowo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fehbvm.com/Article/details/gmicugaib.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gzithmddf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.zdbjq.cn/Article/details/goxibuwya.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gmsbfmstt.sHtML

[S49] C++：写文件
来源：http://3g.fehbvm.com/Article/details/ghylznadw.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fehbvm.com/Article/details/giuqyyhmp.sHtML

[S50] C++：格式化数字
来源：http://www.share.zdbjq.cn/Article/details/gserbcuxo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.hesvh.cn/Article/details/glnrjnbzf.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/gedfxcmup.sHtML

static_cast<double>(a) / b
来源：http://www.blog.hesvh.cn/Article/details/gvxoydouf.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/gxuxvndro.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fehbvm.com/Article/details/goycdzktz.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/gchjzpafj.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/gbdxfbkoz.sHtML

[S54] C++：异常处理
来源：http://wap.zdbjq.cn/Article/details/gghxysyat.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fehbvm.com/Article/details/gilqunofj.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/ggfveqqfg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.zdbjq.cn/Article/details/gsqnsnroz.sHtML

[S56] C++：optional
来源：http://www.blog.zdbjq.cn/Article/details/gjfekswqg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/gjsskutie.sHtML

[S57] C++：编译期常量
来源：http://read.share.fehbvm.com/Article/details/gzfojdagz.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/girgggelk.sHtML

[S58] C++：命名空间
来源：http://3g.zdbjq.cn/Article/details/gibxejnvs.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/gipudsiww.sHtML

[S59] C++：静态断言
来源：http://read.share.fehbvm.com/Article/details/gebjguvtg.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fehbvm.com/Article/details/gitiarpen.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/ghmdicefn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.hesvh.cn/Article/details/gguhqyocc.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqrutupna.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/gixpqanwk.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghcabdcjf.sHtML

[T01] Kotlin：Hello World
来源：http://3g.zdbjq.cn/Article/details/glzxhisti.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gbgzczoeu.sHtML

[T02] Kotlin：变量
来源：http://mobile.hesvh.cn/Article/details/guzkvhhwh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.hesvh.cn/Article/details/gwgnohgxr.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.hesvh.cn/Article/details/gvvpzpdfv.sHtML

"值: $b"
来源：http://blog.hesvh.cn/Article/details/godkmqlkm.sHtML

[T04] Kotlin：空安全
来源：http://read.share.hesvh.cn/Article/details/gjdoxwcpq.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/gynmptjba.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fehbvm.com/Article/details/gnkfdubsr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fehbvm.com/Article/details/gzmxmutos.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/gmoqfzdfw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fehbvm.com/Article/details/gohayfixe.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.hesvh.cn/Article/details/gxrvpvsbi.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fehbvm.com/Article/details/ghhvwkwew.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/gmlulywti.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gjhhffned.sHtML


<!-- 参考信息 -->