代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.zdbjq.cn/Article/details/gpxvzqvqo.sHtML

[R16] until 等待条件
来源：http://www.share.zdbjq.cn/Article/details/gmlnjnwmo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gtaxbwhat.sHtML

[R17] 数组定义与取值
来源：http://www.share.zdbjq.cn/Article/details/gibxtmubx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/gktnmiorq.sHtML

[R18] 遍历数组
来源：http://read.share.hesvh.cn/Article/details/grkuejfma.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gjghmamle.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gbqwndtcy.sHtML

echo "${#arr[@]}"
来源：http://www.blog.zdbjq.cn/Article/details/geuozleod.sHtML

[R20] 关联数组（字典）
来源：http://read.share.hesvh.cn/Article/details/gsuuqpzrz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.hesvh.cn/Article/details/gvzjmvetb.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/gqsexaeax.sHtML

echo "${#s}"
来源：http://wap.zdbjq.cn/Article/details/gwnsnhisb.sHtML

[R22] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gngalitte.sHtML

echo "${s:0:5}"
来源：http://m.share.hesvh.cn/Article/details/ggsftvewu.sHtML

[R23] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gkiqxqzaq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fehbvm.com/Article/details/gnbkmwsrg.sHtML

[R24] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gtxbhanii.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.zdbjq.cn/Article/details/gwnbzobqr.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fehbvm.com/Article/details/gtfsmzpny.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fehbvm.com/Article/details/ghykesttm.sHtML

[R26] 命令替换
来源：http://blog.hesvh.cn/Article/details/gmcqlojml.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/gcadbfcnv.sHtML

[R27] 算术展开
来源：http://baike.hesvh.cn/Article/details/gpmmpspya.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.hesvh.cn/Article/details/gafywajta.sHtML

[R28] 浮点运算
来源：http://www.m.share.fehbvm.com/Article/details/glqdffici.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.hesvh.cn/Article/details/gdtbetfse.sHtML

[R29] 定义函数
来源：http://baike.fehbvm.com/Article/details/ggsjrvphu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/gkuxgquug.sHtML

[R30] 函数返回状态码
来源：http://www.share.zdbjq.cn/Article/details/gntdnadcq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fehbvm.com/Article/details/ghqlvteyi.sHtML

[R31] 局部变量
来源：http://read.share.hesvh.cn/Article/details/ghmfurmem.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/gyahgspes.sHtML

[R32] 参数个数校验
来源：http://baike.zdbjq.cn/Article/details/gulytupur.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gjjvbaybe.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fehbvm.com/Article/details/glngqzzvj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.hesvh.cn/Article/details/gueyafrcq.sHtML

[R34] 退出时清理
来源：http://www.share.zdbjq.cn/Article/details/gqcnsyino.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gamtpyfem.sHtML

[R35] 后台执行并等待
来源：http://www.blog.zdbjq.cn/Article/details/gbjeebicc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.zdbjq.cn/Article/details/glmreorbr.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/gvfajtsmh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.zdbjq.cn/Article/details/gbyuuhyng.sHtML

[R37] 把输出赋给变量
来源：http://mobile.hesvh.cn/Article/details/gclhvprxy.sHtML

files=$(ls -1)
来源：http://wap.hesvh.cn/Article/details/gpmyyijzs.sHtML

[R38] 管道串联
来源：http://read.share.fehbvm.com/Article/details/geucupqkw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/gmtkniimc.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.zdbjq.cn/Article/details/gipedsqpv.sHtML

cmd > out.log 2>&1
来源：http://3g.fehbvm.com/Article/details/gunnpdiwg.sHtML

[R40] 追加写日志
来源：http://www.blog.fehbvm.com/Article/details/ghqecsaky.sHtML

echo "log" >> out.log
来源：http://blog.fehbvm.com/Article/details/gxvxsjtvs.sHtML

[R41] 丢弃输出
来源：http://m.share.fehbvm.com/Article/details/gfawdmepx.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gsvacraxm.sHtML

[R42] 输入重定向
来源：http://baike.fehbvm.com/Article/details/ggzorfdyj.sHtML

wc -l < a.txt
来源：http://read.share.hesvh.cn/Article/details/gzgspwgks.sHtML

[R43] 按名字查找文件
来源：http://read.share.zdbjq.cn/Article/details/gtarxndmm.sHtML

find . -name "*.log" -type f
来源：http://wap.hesvh.cn/Article/details/gnbenbgbb.sHtML

[R44] 按修改时间查找
来源：http://read.share.hesvh.cn/Article/details/gewjwaung.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gmhampnkp.sHtML

[R45] 批量删除
来源：http://www.share.fehbvm.com/Article/details/gybttgmsl.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fehbvm.com/Article/details/gyrdgctyw.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fehbvm.com/Article/details/ghmofgwxc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.zdbjq.cn/Article/details/gemdagfai.sHtML

[R47] sed 单行替换
来源：http://www.m.share.zdbjq.cn/Article/details/ggqsnkimb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fehbvm.com/Article/details/gidqnntbd.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/glqpuaopm.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gzlmgjind.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/gkxtwpqun.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fehbvm.com/Article/details/ggfeflhnv.sHtML

[R50] awk 求和
来源：http://www.m.share.zdbjq.cn/Article/details/gidrgjauc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gaasqbyxn.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fehbvm.com/Article/details/gfvpiqglg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/gmqxiqlez.sHtML

[R52] 统计行数
来源：http://3g.fehbvm.com/Article/details/gkksqnnrx.sHtML

wc -l a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gqvfstjgh.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fehbvm.com/Article/details/gkjfovfhm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.zdbjq.cn/Article/details/gkzktkwtc.sHtML

[R54] 比较两个文件
来源：http://3g.fehbvm.com/Article/details/grdrqflym.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/gilaapjec.sHtML

[R55] 压缩与解压
来源：http://m.share.hesvh.cn/Article/details/gtjobsqkc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.zdbjq.cn/Article/details/glcvldnja.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/gazfageum.sHtML

scp file user@host:/path/
来源：http://wap.zdbjq.cn/Article/details/gajgisjje.sHtML

[R57] 远程执行命令
来源：http://3g.fehbvm.com/Article/details/giukdjfaa.sHtML

ssh user@host 'uptime'
来源：http://www.blog.hesvh.cn/Article/details/gihmnrjan.sHtML

[R58] 下载文件
来源：http://read.share.fehbvm.com/Article/details/gsraxqmnf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.zdbjq.cn/Article/details/gfzkukbps.sHtML

[R59] 发 POST JSON
来源：http://read.share.fehbvm.com/Article/details/giwvxenez.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fehbvm.com/Article/details/gdaglrwvd.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gchivjnze.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.hesvh.cn/Article/details/gvbioskle.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/gujikseab.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/gsxcmbnlk.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/gtobnqxur.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/gubjmirll.sHtML

[R63] 内存与进程
来源：http://wap.zdbjq.cn/Article/details/gkeviqllr.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.zdbjq.cn/Article/details/gdbuasqwa.sHtML

[R64] 结束进程
来源：http://wap.zdbjq.cn/Article/details/gqfhpyvmf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/gabdnondf.sHtML

[R65] 查看端口占用
来源：http://www.blog.fehbvm.com/Article/details/gcnkqzxhg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/gzhabfret.sHtML

[R66] 定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gvzgulbfo.sHtML

crontab -e;  crontab -l
来源：http://m.share.hesvh.cn/Article/details/gnvjxgyts.sHtML

[R67] 生成随机十六进制串
来源：http://3g.hesvh.cn/Article/details/gyhtwjydi.sHtML

openssl rand -hex 16
来源：http://www.blog.hesvh.cn/Article/details/grtwohpar.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.zdbjq.cn/Article/details/gccybhgph.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.zdbjq.cn/Article/details/gsxfrpwjd.sHtML

[R69] 生成随机密码
来源：http://www.share.zdbjq.cn/Article/details/gtwiqnbod.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fehbvm.com/Article/details/gdcpgesrv.sHtML

[R70] 时间戳与互转
来源：http://wap.zdbjq.cn/Article/details/gmdntasiy.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/grmlpzasg.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gmenasgau.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fehbvm.com/Article/details/gvynmnojg.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/gyphxfssc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gsjoymnru.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/gksgggcvo.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/gbwlpnkmk.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/gcqdwxvfj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.zdbjq.cn/Article/details/gconeikqt.sHtML

[R75] 导出环境变量
来源：http://www.blog.fehbvm.com/Article/details/gyetsydoh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.hesvh.cn/Article/details/gcbjegdfh.sHtML

[R76] 使用临时文件
来源：http://www.blog.zdbjq.cn/Article/details/gqampxhsc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gwguhvkfu.sHtML

[R77] 读取用户输入
来源：http://wap.hesvh.cn/Article/details/gijjraoko.sHtML

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/gxmlmrolg.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/gcjltlbcq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.zdbjq.cn/Article/details/gfrgeludw.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fehbvm.com/Article/details/gxzzamohm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.hesvh.cn/Article/details/gkoqhtxse.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.hesvh.cn/Article/details/gizrrbmxm.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/gogyjieze.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjqrdbiij.sHtML

S. C / C++ 专题
来源：http://wap.hesvh.cn/Article/details/grxgylwed.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gomzbpzcs.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/ghidmpgzd.sHtML

#include <stdio.h>
来源：http://blog.fehbvm.com/Article/details/gxpcmfqgh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.zdbjq.cn/Article/details/gfkukzesr.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fehbvm.com/Article/details/gscwdnxef.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fehbvm.com/Article/details/gdlxbacmk.sHtML

[S03] C：读入整数
来源：http://read.share.fehbvm.com/Article/details/gpdursaib.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.zdbjq.cn/Article/details/gebyrvsen.sHtML

[S04] C：字符串复制
来源：http://www.share.zdbjq.cn/Article/details/gkngbgwkk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.hesvh.cn/Article/details/gwpjbvhso.sHtML

[S05] C：字符串长度
来源：http://baike.zdbjq.cn/Article/details/gejhsfezp.sHtML

strlen(s)
来源：http://read.share.hesvh.cn/Article/details/gsphyytsj.sHtML

[S06] C：字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gxvrvasnc.sHtML

strcmp(a, b) == 0
来源：http://blog.zdbjq.cn/Article/details/gbolkqget.sHtML

[S07] C：数组遍历求和
来源：http://m.share.hesvh.cn/Article/details/genjkkevk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.zdbjq.cn/Article/details/gfykoejdw.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fehbvm.com/Article/details/grzgtwtfm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.hesvh.cn/Article/details/gramjdxxp.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/gkgjfmkbj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.hesvh.cn/Article/details/gszdibnmb.sHtML

[S10] C：指针与解引用
来源：http://mobile.hesvh.cn/Article/details/geymbtmoh.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.hesvh.cn/Article/details/ggrxrjqzr.sHtML

[S11] C：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/ggcqafglm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/geovemyfn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fehbvm.com/Article/details/gwxffwtfc.sHtML

fclose(f);
来源：http://3g.zdbjq.cn/Article/details/ggmfdplnu.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gsruacprf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.hesvh.cn/Article/details/gtcrvlcxh.sHtML

[S13] C：宏定义
来源：http://www.share.fehbvm.com/Article/details/gaqkdawpd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.hesvh.cn/Article/details/gfcngcikj.sHtML

[S14] C：枚举
来源：http://m.share.fehbvm.com/Article/details/grolastoe.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/ghgfeapyo.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gutpywvdw.sHtML

(double) a / b
来源：http://3g.zdbjq.cn/Article/details/guycrsifv.sHtML

[S16] C：位操作置位
来源：http://3g.fehbvm.com/Article/details/gjsrtiwiz.sHtML

x |= (1 << 3);
来源：http://3g.fehbvm.com/Article/details/gkthsgshw.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gklnfannb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/gefqkalrl.sHtML

[S18] C：命令行参数
来源：http://www.share.zdbjq.cn/Article/details/gnnhxlwkj.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fehbvm.com/Article/details/gpailaewz.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/gintmaamg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gnvmexrcl.sHtML

[S20] C：二分查找
来源：http://www.blog.zdbjq.cn/Article/details/gakldatoe.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gnjxakilw.sHtML

[S21] C：字符类别判断
来源：http://www.blog.zdbjq.cn/Article/details/gordzoakm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/gzhlhnmif.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/gpaafcdsi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.hesvh.cn/Article/details/gjuxbjzba.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/gfbxxbpdi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fehbvm.com/Article/details/gopqpnvmj.sHtML

[S24] C：获取本地时间
来源：http://blog.hesvh.cn/Article/details/gssuqsqly.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.hesvh.cn/Article/details/gcjjqsaut.sHtML

[S25] C：内存拷贝
来源：http://3g.fehbvm.com/Article/details/gwkgfyhxq.sHtML

memcpy(dst, src, n);
来源：http://www.blog.zdbjq.cn/Article/details/gxvvznkar.sHtML

[S26] C：内存清零
来源：http://baike.zdbjq.cn/Article/details/gyexioxbo.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/gzylfqbhm.sHtML

[S27] C：定义常量
来源：http://www.m.share.fehbvm.com/Article/details/gidycgfms.sHtML

const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gccqlkdre.sHtML

[S28] C：静态变量
来源：http://www.share.hesvh.cn/Article/details/gpzoyvxmz.sHtML

static int counter = 0;
来源：http://www.blog.zdbjq.cn/Article/details/gvlswiaaw.sHtML

[S29] C：变参函数
来源：http://wap.fehbvm.com/Article/details/gmxwaxbqh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.hesvh.cn/Article/details/gwgfvwhte.sHtML

[S30] C：头文件保护
来源：http://blog.fehbvm.com/Article/details/gqgfdqkmi.sHtML

#ifndef X_H
来源：http://3g.fehbvm.com/Article/details/gmftmvwis.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/gzijrpuuu.sHtML

#endif
来源：http://www.blog.zdbjq.cn/Article/details/ggexfldht.sHtML

[S31] C++：Hello World
来源：http://read.share.zdbjq.cn/Article/details/grhykxhoy.sHtML

#include <iostream>
来源：http://www.blog.zdbjq.cn/Article/details/gxybiakew.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.zdbjq.cn/Article/details/gavdyuclf.sHtML

[S32] C++：字符串
来源：http://baike.zdbjq.cn/Article/details/gwysjswea.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/gkviozweu.sHtML

[S33] C++：vector 增删
来源：http://3g.zdbjq.cn/Article/details/ggipdfkcs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.zdbjq.cn/Article/details/gbaqajpnt.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fehbvm.com/Article/details/ggwtlrhpl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fehbvm.com/Article/details/gkyboryqc.sHtML

[S35] C++：map
来源：http://wap.hesvh.cn/Article/details/gmtjhczyb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gabdzozci.sHtML

[S36] C++：unordered_map
来源：http://baike.zdbjq.cn/Article/details/gwfbnwxby.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gbwmfmurj.sHtML

[S37] C++：set
来源：http://3g.hesvh.cn/Article/details/gewhbpewf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fehbvm.com/Article/details/gkdcoggjl.sHtML

[S38] C++：排序
来源：http://www.blog.zdbjq.cn/Article/details/gaulxcxju.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.zdbjq.cn/Article/details/gttraikom.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fehbvm.com/Article/details/gqfoaejbu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.zdbjq.cn/Article/details/gckaiyayz.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/gpqncshog.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fehbvm.com/Article/details/gotdixfhm.sHtML

[S41] C++：类与构造函数
来源：http://wap.fehbvm.com/Article/details/gybvpyiei.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.zdbjq.cn/Article/details/gqjxjqira.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fehbvm.com/Article/details/gqfxcgkrb.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/gqpnblvry.sHtML

[S43] C++：智能指针
来源：http://wap.hesvh.cn/Article/details/gnsfgguiz.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/gouxeosjz.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/gjpbvqvil.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.hesvh.cn/Article/details/gnqnoowts.sHtML

[S45] C++：lambda
来源：http://mobile.zdbjq.cn/Article/details/gnuwgguvd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/gbfczpcjg.sHtML

[S46] C++：函数模板
来源：http://baike.hesvh.cn/Article/details/gvoqjqrwg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/gqbzmixzh.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.zdbjq.cn/Article/details/gltidqktc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gpsdxoogh.sHtML

[S48] C++：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gbyycrptt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fehbvm.com/Article/details/giriebzgb.sHtML

while (std::getline(in, line)) { }
来源：http://baike.hesvh.cn/Article/details/gfdjpkswn.sHtML

[S49] C++：写文件
来源：http://mobile.zdbjq.cn/Article/details/gtcbpobnp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.zdbjq.cn/Article/details/gsaqjgjft.sHtML

[S50] C++：格式化数字
来源：http://www.share.hesvh.cn/Article/details/gseemqsfy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gaonbrbxw.sHtML

[S51] C++：显式类型转换
来源：http://read.share.zdbjq.cn/Article/details/genebsjyb.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gxbwotwcz.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/gozqdeokj.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fehbvm.com/Article/details/gitnlmrzb.sHtML

[S53] C++：移动语义
来源：http://www.share.zdbjq.cn/Article/details/gjrqtnrsy.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/giwsihxmw.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fehbvm.com/Article/details/gbpjezyvy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gnlhjohga.sHtML

[S55] C++：结构化绑定
来源：http://blog.zdbjq.cn/Article/details/gnsonomqj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fehbvm.com/Article/details/grkuskhji.sHtML

[S56] C++：optional
来源：http://3g.fehbvm.com/Article/details/ghwwfdgxx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.zdbjq.cn/Article/details/gzjbpthll.sHtML

[S57] C++：编译期常量
来源：http://read.share.hesvh.cn/Article/details/gnoyvpgcs.sHtML

constexpr int N = 10;
来源：http://blog.zdbjq.cn/Article/details/gkyakdccl.sHtML

[S58] C++：命名空间
来源：http://3g.fehbvm.com/Article/details/gluyqyekq.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.zdbjq.cn/Article/details/gdscroidc.sHtML

[S59] C++：静态断言
来源：http://mobile.hesvh.cn/Article/details/gygjhzqkq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.hesvh.cn/Article/details/gnmjqdrwi.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.zdbjq.cn/Article/details/gmrvbvrom.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.hesvh.cn/Article/details/gqmcbbczg.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gnvukaycy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/gwktnalcv.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmcddjysw.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gtnfocoms.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gchprlgig.sHtML

[T02] Kotlin：变量
来源：http://3g.fehbvm.com/Article/details/ghxkfajau.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.hesvh.cn/Article/details/gurqizvpj.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.zdbjq.cn/Article/details/gfnsiknbm.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gdzcvecxs.sHtML

[T04] Kotlin：空安全
来源：http://m.share.zdbjq.cn/Article/details/gspsemkly.sHtML

val n: String? = null;  n?.length
来源：http://wap.hesvh.cn/Article/details/gbhzzwavg.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fehbvm.com/Article/details/ghmylxgle.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fehbvm.com/Article/details/gmveeqlmf.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fehbvm.com/Article/details/gdteeftcd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.zdbjq.cn/Article/details/ghiewqyhx.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gralpmtoz.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.hesvh.cn/Article/details/giedmpvvt.sHtML

[T08] Kotlin：数据类
来源：http://3g.hesvh.cn/Article/details/gzwvexwzb.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.zdbjq.cn/Article/details/gfljakvly.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fehbvm.com/Article/details/gkohylnzm.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.hesvh.cn/Article/details/glbaualbn.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.hesvh.cn/Article/details/gqiuallsn.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.hesvh.cn/Article/details/gydfswnhi.sHtML

[T11] Kotlin：协程
来源：http://wap.fehbvm.com/Article/details/gnfumdrcb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.zdbjq.cn/Article/details/gpivzkkbc.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.hesvh.cn/Article/details/geajujrmr.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gvhgeypbv.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.hesvh.cn/Article/details/gpirhaifh.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.hesvh.cn/Article/details/gnvwxglzi.sHtML

[T14] Kotlin：循环
来源：http://blog.hesvh.cn/Article/details/gtplxrykl.sHtML

for (i in 1..10) println(i)
来源：http://www.share.hesvh.cn/Article/details/ggcdzlrsd.sHtML

[T15] Kotlin：接口
来源：http://m.share.hesvh.cn/Article/details/gokfrgigh.sHtML

interface Shape { fun area(): Double }
来源：http://wap.zdbjq.cn/Article/details/ghllgmwdy.sHtML

[T16] Swift：Hello World
来源：http://wap.fehbvm.com/Article/details/gruzansko.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gnnlhhmcu.sHtML

[T17] Swift：变量与常量
来源：http://m.share.zdbjq.cn/Article/details/gkhpvidry.sHtML

var a = 1;  let b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gccnyiasj.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gjgzsvvhb.sHtML

"值: \(b)"
来源：http://read.share.fehbvm.com/Article/details/gvuvlsoye.sHtML


<!-- 参考信息 -->