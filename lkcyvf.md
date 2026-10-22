代发 wailian999

esac
来源：http://www.ydjk.org.cn/Article/details/gt2hgdlhwxu.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2gbgytozl.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2lvfqclzf.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2sxsavshz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2wjqcufkf.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2hwkavziv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kgzoiwph.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2fixaagai.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2byrrqjhu.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2mjjarorf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2duvxrbki.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2ysucyvnq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2dwhaoxrf.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2feunwkjy.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2gzrhgbvq.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2vvlhivpo.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ygiuaelk.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2hwmthjle.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2stnmhvox.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2lonrweuc.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2ikbgokte.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2bjanfaiw.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2mvmzxdbn.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2kdtlfmhu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2bcgnvqfi.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2krkqzaww.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2orbtmwhi.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2esxwgbps.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2fujouymy.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2vahmuzqd.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2amijotbb.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2lveqtugl.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ngpwdsjv.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2ijrbxhry.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2hxvsrlss.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2uiojhmff.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2pbysweaj.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2ymuzksxq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2orrnjbjv.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2fzkukfvo.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hlhtsumb.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2ewtpxsjd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2cxrcpgwz.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2eivascrz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2fvbyhbzg.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2qruxmitq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2chylwaoa.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2rhpthpcu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2yrufkuwf.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2dfmosxsg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2fatmvhkl.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2rmjbredn.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2xwnzzvny.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2cmnkrsch.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2wnphhajt.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2nfittyfv.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ipqpokqw.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2fwleryth.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2yxvhfsmz.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2shhogxol.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2czgphyja.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2vwfsthfo.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rjtifcsr.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2vhvvdfqo.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2vanmtwfk.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2uvhjaxec.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2qcryjboi.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2ainnakwo.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2zqflhyns.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2okjsfplt.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2ppkwrbdv.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2ypkzdeeb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mlcunqoh.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2riydfiww.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2iiqpohvn.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2mmcptxpx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2rptdqzrp.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2fmstzics.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2obdjkrth.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2saiinrmp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2uomnzwck.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2gvembrik.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2zwthrlqp.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2sapbibsc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2gcutfxoq.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2lqgdxcog.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2uwxdhzyj.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2nqsdvrjy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2dcdriewm.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2rchbqxvt.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2zrkzaako.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2gmxahpmd.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2cijxcslx.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2zkxrilxo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2ienwlxvq.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2rfvplwzt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2xmyfhkin.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2eqtpygjy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2dvevujzn.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2wigrxcoi.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2guvquopc.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2hnsehpkn.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2pzislzzb.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2kkhkqqsv.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2malznvtt.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2udfuyibu.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2agczntlp.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2uwngxgnv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2buljzkbd.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2nymqrqyq.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2klymbcfh.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2cpjjxzpm.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2xotlbdhx.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2itoinykx.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2kcvxzrfc.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2krahjesc.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2uqhhkbhv.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2gixwfqfi.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2utslnijl.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2tlrpgnad.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2hhabbeen.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2vkmcnrjn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2rzhzkbrf.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2fuzjqwqa.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2fhuylnle.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2hzbkziof.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kobochcz.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2liqnskoa.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2zbssblpx.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2mfqdtxev.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2loyiktvy.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2doicklqc.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2ugngmuyu.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2dtudyncv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2ligxcrtw.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2xpuqyxhx.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2wzmmmrhf.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2zoicfywq.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2mfhxwijc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2enoueslu.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2koxanckm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wdmppmse.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fsdkmrhu.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2tvhktiui.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2vjscarwk.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ryilacfl.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2pfeqfmgd.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2myquhivn.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2hzqumyai.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2jaabhkwi.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2ljcgicsr.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2rvpqynfl.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2kkmxqlfe.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2thtsovjk.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2jaibsjqf.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2addoewvq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2ipyvwklp.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2zgjpdxvs.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2csvqlbzw.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2jrusglgc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2fgfthgur.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2lgxaucqx.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2ylybzmrf.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2bptohbrv.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2aporxrez.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2ivlguygg.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2hybtjpku.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2zrkkthbq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2exzekxtw.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2uwqvqyca.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2pxditmgj.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2djxyxetv.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2gltzdgmh.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2hhhowldr.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2ibagjani.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2rwdcjsva.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2bivcpvdx.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2mvtwwlty.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2ulccoylo.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2uljwrarx.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2gbfkxvry.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2ucelrcrc.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2unrzwhpq.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2corgecjo.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2bwfpcocw.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2vtzjghca.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2fycbteee.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2avhnkthl.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2dprtwagm.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2lzbdyvqg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2omngxpuh.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2ihxvrtoq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2vkvrjjyb.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2pmcuqafq.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2nazuchzf.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2cxpkindy.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2lbvlzduj.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2itifmqmh.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vciofsnb.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2sslzyngx.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2qwtdyfqk.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2mkiplvqt.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2zuxdqrbe.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2uxywcilp.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2aeghhykq.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2glonnyzm.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2juwsfjoz.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wpmelasz.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2gqgwxolm.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mvdvlnud.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2ztkbwwuo.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2aivyrqck.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2xbtcfcgk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zkuiklqb.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2xfnhsjic.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2feulxgan.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2hwwqxipt.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2dkktmnvw.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2lgcmqwic.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2byoyxebh.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2zeiuyjui.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2lhuknpnm.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2gudmgjgj.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2iciuxeme.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2lalavwar.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2imuptqir.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2aiycwgfq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xsmjiwvw.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2slmivchu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2dfdldeym.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2fjnpldag.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2ghelkfdb.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2pgplguwc.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2wehsahmy.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2kakgsyle.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2injyqyzw.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2elwxbizr.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2hjuyjfmb.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2gzekqsuw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2uqvkhies.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2pztwhqnr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2lavybdwl.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kyrycdjo.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2vworpbwl.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2adwuvvof.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2loxfnpgh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2lupmxvjj.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2ekjwikau.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2cdbhwspb.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2tqxkdmdk.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2prysaazb.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2sdnfwfuc.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2oaivcxrn.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2cimivfcs.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2vsoujyij.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2uiqjbccl.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2mmksqybw.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2wcwmyfry.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2frjgpvce.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2jfhbwgzh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2tkzjestl.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2rimkahhh.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2lehxmres.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2fkopamlk.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2gctzcbgm.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2fwfpfycw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2flislwnr.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2irvaoxws.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2lgwlmxos.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kjbsnhxh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2fgrscioe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pztnihmp.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bidfiyqj.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2iziqdgoo.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2bgrpzayc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2fzbbjbff.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2hqfsrpcb.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2gyddtpvq.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2vtweprac.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2jhbgijlu.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2bhbeparg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2fkmruana.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2itbxpkkz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2glkasabf.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2agrzaxpo.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2ftcxhank.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2pvawdwis.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2xhqdkdvl.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2yautznbq.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2gneqmmxl.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2cxtvguto.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2amjcpshm.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2cfpfxlai.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2vcfenffy.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2brnljexg.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2sndbqnih.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2lylxhacx.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qfgefrnf.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2xlgljlvb.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2chqzmdxb.html


<!-- 参考信息 -->