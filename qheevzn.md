代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.hesvh.cn/Article/details/gzxcyyrax.sHtML

[R26] 命令替换
来源：http://mobile.zdbjq.cn/Article/details/gwkolrczj.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.zdbjq.cn/Article/details/gtpojojmo.sHtML

[R27] 算术展开
来源：http://read.share.zdbjq.cn/Article/details/gqmyvorrx.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/goxtglnag.sHtML

[R28] 浮点运算
来源：http://wap.fehbvm.com/Article/details/gsazdhrqm.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fehbvm.com/Article/details/gcfvooaou.sHtML

[R29] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gamlybmiy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fehbvm.com/Article/details/gueudvxcv.sHtML

[R30] 函数返回状态码
来源：http://3g.fehbvm.com/Article/details/grnjyzchd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.zdbjq.cn/Article/details/gcmttoxoy.sHtML

[R31] 局部变量
来源：http://wap.fehbvm.com/Article/details/gyxapcwzw.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fehbvm.com/Article/details/gsysrzcqu.sHtML

[R32] 参数个数校验
来源：http://blog.zdbjq.cn/Article/details/gfkdsbxax.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gehwimtwq.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.hesvh.cn/Article/details/ghnjqfiwn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fehbvm.com/Article/details/gfcqbzbnt.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/gqghwwokl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gmcfdirij.sHtML

[R35] 后台执行并等待
来源：http://baike.zdbjq.cn/Article/details/grosvpqzn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.hesvh.cn/Article/details/gjgozjhsg.sHtML

[R36] 并发执行多个任务
来源：http://baike.hesvh.cn/Article/details/gekohyxtq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fehbvm.com/Article/details/gbrrclbvr.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fehbvm.com/Article/details/gkyjtplfk.sHtML

files=$(ls -1)
来源：http://www.m.share.hesvh.cn/Article/details/gnljmhfds.sHtML

[R38] 管道串联
来源：http://www.m.share.hesvh.cn/Article/details/gfecgpjoc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/gsuytvjev.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.zdbjq.cn/Article/details/gbxtduhis.sHtML

cmd > out.log 2>&1
来源：http://3g.fehbvm.com/Article/details/gsyizimmr.sHtML

[R40] 追加写日志
来源：http://m.share.fehbvm.com/Article/details/gctwqbhme.sHtML

echo "log" >> out.log
来源：http://www.blog.hesvh.cn/Article/details/gjokymvxq.sHtML

[R41] 丢弃输出
来源：http://m.share.fehbvm.com/Article/details/gnjyiqsrh.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gbyivlngi.sHtML

[R42] 输入重定向
来源：http://read.share.fehbvm.com/Article/details/gqjnyhxxc.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gkxllxixs.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/gdrhfwrxl.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/ghnfuhbdt.sHtML

[R44] 按修改时间查找
来源：http://3g.hesvh.cn/Article/details/gaqxttgrw.sHtML

find . -mtime -7 -type f
来源：http://wap.hesvh.cn/Article/details/gmlwknqfr.sHtML

[R45] 批量删除
来源：http://www.m.share.zdbjq.cn/Article/details/gdwmcudwb.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fehbvm.com/Article/details/gabupnqav.sHtML

[R46] 递归替换文件内容
来源：http://mobile.zdbjq.cn/Article/details/gypfhlixk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fehbvm.com/Article/details/goflfdzzr.sHtML

[R47] sed 单行替换
来源：http://3g.hesvh.cn/Article/details/ghdlpfumu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gztunuvjr.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/gwzhixrvs.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gztcznrzj.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/gbetonlmd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/gosmmjrgi.sHtML

[R50] awk 求和
来源：http://3g.hesvh.cn/Article/details/gsivbokwu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.zdbjq.cn/Article/details/govivibnb.sHtML

[R51] 排序去重取前几
来源：http://www.blog.hesvh.cn/Article/details/greginmfb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fehbvm.com/Article/details/gvufussgg.sHtML

[R52] 统计行数
来源：http://www.blog.fehbvm.com/Article/details/gurgsunan.sHtML

wc -l a.txt
来源：http://www.share.fehbvm.com/Article/details/ggfmscben.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fehbvm.com/Article/details/gvmhyzhzb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.hesvh.cn/Article/details/gyfyhyizk.sHtML

[R54] 比较两个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gjzpzvzgn.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/gwalvyetx.sHtML

[R55] 压缩与解压
来源：http://3g.zdbjq.cn/Article/details/gmsdlhjye.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.hesvh.cn/Article/details/gxrxsweul.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/geuosvllw.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/gzezpvacl.sHtML

[R57] 远程执行命令
来源：http://www.blog.fehbvm.com/Article/details/ggrvrpizp.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.hesvh.cn/Article/details/getjmivqw.sHtML

[R58] 下载文件
来源：http://m.share.zdbjq.cn/Article/details/gqjgbdfnx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.zdbjq.cn/Article/details/gualzykyc.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gvkdpdysc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.zdbjq.cn/Article/details/gssnedvsd.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gzjwstkjx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.zdbjq.cn/Article/details/gssjtrurm.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/gwoyxxxmd.sHtML

df -h;  du -sh *
来源：http://baike.zdbjq.cn/Article/details/gekkaogzv.sHtML

[R62] 找最占空间的文件
来源：http://baike.zdbjq.cn/Article/details/gqnzgzngg.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.hesvh.cn/Article/details/gbokajzed.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/gavbpklsg.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/gbrgzrfgh.sHtML

[R64] 结束进程
来源：http://baike.fehbvm.com/Article/details/gwqvngbdo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/gwckjpeec.sHtML

[R65] 查看端口占用
来源：http://mobile.zdbjq.cn/Article/details/gbhbwxjcw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.zdbjq.cn/Article/details/gitosejxn.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/ggrnvqfqf.sHtML

crontab -e;  crontab -l
来源：http://wap.hesvh.cn/Article/details/gjcpnrois.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.zdbjq.cn/Article/details/gvgeqxaqe.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/gmmmzxhvp.sHtML

[R68] 计算文件校验值
来源：http://3g.fehbvm.com/Article/details/gtasweugx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.hesvh.cn/Article/details/gvwldghni.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/gykxumjju.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/gsztemaxr.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/gxatkisjp.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/gwsmaetzw.sHtML

[R71] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gzuplbbaj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/gickcjvnj.sHtML

[R72] 等待端口就绪
来源：http://m.share.zdbjq.cn/Article/details/ghkvueeek.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gantkrozo.sHtML

[R73] 分割大日志
来源：http://www.m.share.fehbvm.com/Article/details/glivtesco.sHtML

split -l 1000 big.log part_
来源：http://read.share.hesvh.cn/Article/details/gptlxhmxn.sHtML

[R74] 批量重命名
来源：http://www.share.fehbvm.com/Article/details/gzghuykmo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/greaayudh.sHtML

[R75] 导出环境变量
来源：http://www.share.hesvh.cn/Article/details/gxgmxuxul.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.hesvh.cn/Article/details/gfxeemurx.sHtML

[R76] 使用临时文件
来源：http://baike.hesvh.cn/Article/details/gzgarwbzo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gfoflfsxd.sHtML

[R77] 读取用户输入
来源：http://blog.hesvh.cn/Article/details/gyyysnpzj.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/gvaqrxfsy.sHtML

[R78] 交互式菜单
来源：http://www.blog.fehbvm.com/Article/details/gkokyivlx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.zdbjq.cn/Article/details/gugtkmlly.sHtML

[R79] 解析命令行选项
来源：http://baike.hesvh.cn/Article/details/gvngjnsul.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.hesvh.cn/Article/details/gkjtsmeiv.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.hesvh.cn/Article/details/gnrndxdhi.sHtML

time ./run.sh
来源：http://www.m.share.hesvh.cn/Article/details/gzsbcdnii.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gnryytweh.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gwhabsfqe.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gsytuetdh.sHtML

[S01] C：Hello World
来源：http://www.share.hesvh.cn/Article/details/gydrndhvj.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/gaumnnxft.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.hesvh.cn/Article/details/gtovlbgpm.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fehbvm.com/Article/details/gjghpwexe.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fehbvm.com/Article/details/gcnoyqkos.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gnmpcemvn.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/gxpgxqujw.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/gpdnlubof.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.hesvh.cn/Article/details/gnlmaasqp.sHtML

[S05] C：字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gocyykupp.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/glgcyuetr.sHtML

[S06] C：字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gzhdqnhbv.sHtML

strcmp(a, b) == 0
来源：http://blog.zdbjq.cn/Article/details/glvujhqls.sHtML

[S07] C：数组遍历求和
来源：http://wap.zdbjq.cn/Article/details/gbqalqysc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.hesvh.cn/Article/details/gunmkpkfv.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fehbvm.com/Article/details/gfxdzgwdm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/grrksqclx.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.hesvh.cn/Article/details/gjkamzmtb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fehbvm.com/Article/details/gutaquqmo.sHtML

[S10] C：指针与解引用
来源：http://3g.zdbjq.cn/Article/details/gjwhmtlyu.sHtML

int *p = &a;  *p = 5;
来源：http://blog.hesvh.cn/Article/details/gferzrgpx.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gokwoidfx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/gspqvvpms.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gqcmbbwlc.sHtML

fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gngngvwxw.sHtML

[S12] C：写文件
来源：http://m.share.zdbjq.cn/Article/details/gdrkxhoeo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.zdbjq.cn/Article/details/grfmdsfvw.sHtML

[S13] C：宏定义
来源：http://www.blog.fehbvm.com/Article/details/ghwdfpeqp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.hesvh.cn/Article/details/gwnvzjtgs.sHtML

[S14] C：枚举
来源：http://m.share.zdbjq.cn/Article/details/guoadtlbb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.hesvh.cn/Article/details/gqksezbhk.sHtML

[S15] C：类型转换
来源：http://baike.zdbjq.cn/Article/details/glqermukv.sHtML

(double) a / b
来源：http://www.m.share.hesvh.cn/Article/details/gabioiltp.sHtML

[S16] C：位操作置位
来源：http://mobile.hesvh.cn/Article/details/grvhjdcqg.sHtML

x |= (1 << 3);
来源：http://www.share.zdbjq.cn/Article/details/glmcrzrzy.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gcyxzviov.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/gimjgfhga.sHtML

[S18] C：命令行参数
来源：http://3g.fehbvm.com/Article/details/gexjegrrb.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/ggnhfujvd.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/gaficrmcy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gjsywwisl.sHtML

[S20] C：二分查找
来源：http://blog.fehbvm.com/Article/details/gzbczmtee.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gmavtcnqi.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gityudhuy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/gfhktywpk.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/goyvxotte.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.hesvh.cn/Article/details/gnbsksomf.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/gsefxihuc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fehbvm.com/Article/details/grrwzaypf.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/gqruvzpxd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fehbvm.com/Article/details/gilffjzzb.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/ggbgzvywj.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/gocxbiuil.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/gcjitknno.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fehbvm.com/Article/details/gixprotmb.sHtML

[S27] C：定义常量
来源：http://blog.zdbjq.cn/Article/details/gndlakqmj.sHtML

const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/guylvamlc.sHtML

[S28] C：静态变量
来源：http://mobile.fehbvm.com/Article/details/gscsamedi.sHtML

static int counter = 0;
来源：http://www.blog.zdbjq.cn/Article/details/gctrqrhqa.sHtML

[S29] C：变参函数
来源：http://3g.zdbjq.cn/Article/details/gbxpnwwqo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fehbvm.com/Article/details/gtluwztfv.sHtML

[S30] C：头文件保护
来源：http://3g.zdbjq.cn/Article/details/gxvfgbufm.sHtML

#ifndef X_H
来源：http://mobile.hesvh.cn/Article/details/gfusqmhfl.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/gmyklaasv.sHtML

#endif
来源：http://baike.zdbjq.cn/Article/details/glcuxrjbw.sHtML

[S31] C++：Hello World
来源：http://www.share.fehbvm.com/Article/details/gwmtywcgq.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/gqthttmew.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fehbvm.com/Article/details/gjxaciyiz.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/gorjbvorb.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.zdbjq.cn/Article/details/gsmfgyexe.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/gzwnpitfd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fehbvm.com/Article/details/gtipdcrmx.sHtML

[S34] C++：遍历 vector
来源：http://3g.fehbvm.com/Article/details/gnhmqxpbx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.hesvh.cn/Article/details/gjvnkuuyj.sHtML

[S35] C++：map
来源：http://blog.zdbjq.cn/Article/details/goqrxdzqo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gmngkvxtk.sHtML

[S36] C++：unordered_map
来源：http://read.share.fehbvm.com/Article/details/gyxqbxfii.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gixdqowaw.sHtML

[S37] C++：set
来源：http://baike.zdbjq.cn/Article/details/grnldvpwi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.zdbjq.cn/Article/details/garbttynr.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/gzwsicqwh.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fehbvm.com/Article/details/gqudhokuc.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.zdbjq.cn/Article/details/gvhgywgwj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.zdbjq.cn/Article/details/gaateornq.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/gywzohsjj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.zdbjq.cn/Article/details/gidkkowmo.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gqyjnuacf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.zdbjq.cn/Article/details/gqhbvsfvp.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/glqrrblkn.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/gmqbfvosk.sHtML

[S43] C++：智能指针
来源：http://3g.zdbjq.cn/Article/details/ghxusbelr.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fehbvm.com/Article/details/ghszlajxr.sHtML

[S44] C++：引用传参
来源：http://read.share.hesvh.cn/Article/details/gsanymkah.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.hesvh.cn/Article/details/gvodcqstw.sHtML

[S45] C++：lambda
来源：http://m.share.fehbvm.com/Article/details/gvfymdobp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/gyfpatbax.sHtML

[S46] C++：函数模板
来源：http://www.m.share.hesvh.cn/Article/details/gpvylgtwf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.hesvh.cn/Article/details/gxejuphfh.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/gwxrusdob.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.zdbjq.cn/Article/details/glrrhbjga.sHtML

[S48] C++：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gasclsoaj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.hesvh.cn/Article/details/gbginfxhj.sHtML

while (std::getline(in, line)) { }
来源：http://3g.hesvh.cn/Article/details/gizlpatuc.sHtML

[S49] C++：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gtonukmzt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.zdbjq.cn/Article/details/ggxbefswo.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fehbvm.com/Article/details/gpdavcfbu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/gpokxfnjt.sHtML

[S51] C++：显式类型转换
来源：http://mobile.hesvh.cn/Article/details/gbvhblezv.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fehbvm.com/Article/details/ghcbzdews.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/gqehbsyzo.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.zdbjq.cn/Article/details/gdhrlwdcw.sHtML

[S53] C++：移动语义
来源：http://www.m.share.zdbjq.cn/Article/details/gvqbsmrmo.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.zdbjq.cn/Article/details/gtafufatq.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fehbvm.com/Article/details/gtfhyzzlp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fehbvm.com/Article/details/gddqnlnma.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/grcxwlulo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/gjjwqfuzx.sHtML

[S56] C++：optional
来源：http://m.share.hesvh.cn/Article/details/gwkbwvjze.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.zdbjq.cn/Article/details/gzdaashje.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.zdbjq.cn/Article/details/gqxowggbu.sHtML

constexpr int N = 10;
来源：http://3g.zdbjq.cn/Article/details/gteaynnnp.sHtML

[S58] C++：命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gguhtpdfr.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.hesvh.cn/Article/details/gdlxfgyts.sHtML

[S59] C++：静态断言
来源：http://blog.fehbvm.com/Article/details/gxmzotihs.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.hesvh.cn/Article/details/gtjttnllw.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.hesvh.cn/Article/details/gsqtljylg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/gaocbvxqx.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghazieifl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/giukzvaab.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxxyasvlf.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fehbvm.com/Article/details/guyespbkq.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gxjcbcsxu.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/gjmglfejy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.zdbjq.cn/Article/details/ghqltfegj.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.zdbjq.cn/Article/details/gusaryeqi.sHtML

"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gdtvqaqhv.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/gxkyfvxdg.sHtML

val n: String? = null;  n?.length
来源：http://wap.hesvh.cn/Article/details/gmflsqqto.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fehbvm.com/Article/details/grcxkhrnv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.zdbjq.cn/Article/details/ghshahwoj.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gwuhphkhz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/gjcjdkilb.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fehbvm.com/Article/details/gnaxazaaq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.zdbjq.cn/Article/details/gdsazifol.sHtML

[T08] Kotlin：数据类
来源：http://www.share.zdbjq.cn/Article/details/ghivadttu.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/gqkybpqrw.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.hesvh.cn/Article/details/gfiacmsbi.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fehbvm.com/Article/details/glwzmbbyg.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fehbvm.com/Article/details/gqzokfncu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fehbvm.com/Article/details/gnhgnlqpy.sHtML

[T11] Kotlin：协程
来源：http://blog.hesvh.cn/Article/details/guqnvsuad.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fehbvm.com/Article/details/gpcbdchyb.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fehbvm.com/Article/details/gxqkjqehs.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gtjfbgesv.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.hesvh.cn/Article/details/gurbijgfd.sHtML

val m = mapOf("a" to 1)
来源：http://blog.hesvh.cn/Article/details/gmmdxehid.sHtML

[T14] Kotlin：循环
来源：http://mobile.fehbvm.com/Article/details/gouhurhoq.sHtML

for (i in 1..10) println(i)
来源：http://baike.zdbjq.cn/Article/details/gklymbjfh.sHtML

[T15] Kotlin：接口
来源：http://m.share.zdbjq.cn/Article/details/gtbwajuyg.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.hesvh.cn/Article/details/goxzljynv.sHtML

[T16] Swift：Hello World
来源：http://3g.fehbvm.com/Article/details/gakyrgqcl.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gqhhwbkse.sHtML

[T17] Swift：变量与常量
来源：http://3g.fehbvm.com/Article/details/geoxpzokq.sHtML

var a = 1;  let b = 2
来源：http://baike.hesvh.cn/Article/details/gttpvhayw.sHtML

[T18] Swift：字符串插值
来源：http://baike.zdbjq.cn/Article/details/giszgkyzz.sHtML

"值: \(b)"
来源：http://m.share.fehbvm.com/Article/details/ggqqoffdq.sHtML

[T19] Swift：可选绑定
来源：http://www.share.hesvh.cn/Article/details/giwcrwhpf.sHtML

if let n = opt { print(n) }
来源：http://3g.hesvh.cn/Article/details/gklstbkcr.sHtML

[T20] Swift：数组操作
来源：http://www.share.hesvh.cn/Article/details/ghuhgpsjg.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.hesvh.cn/Article/details/gifmgcurj.sHtML

[T21] Swift：遍历
来源：http://blog.fehbvm.com/Article/details/gboqmattz.sHtML

for x in a { print(x) }
来源：http://blog.fehbvm.com/Article/details/gbvczzkof.sHtML

[T22] Swift：字典
来源：http://mobile.zdbjq.cn/Article/details/gioaibvbv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.hesvh.cn/Article/details/gqpxrxkxl.sHtML

[T23] Swift：函数
来源：http://wap.zdbjq.cn/Article/details/gilweipsb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fehbvm.com/Article/details/gyivlsfxi.sHtML

[T24] Swift：闭包
来源：http://m.share.zdbjq.cn/Article/details/gthifuzyo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.hesvh.cn/Article/details/gbmyzgpne.sHtML

[T25] Swift：结构体
来源：http://www.share.hesvh.cn/Article/details/gvjonrqgd.sHtML

struct P { var x: Int }
来源：http://mobile.hesvh.cn/Article/details/gawjjtaih.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fehbvm.com/Article/details/gzezhgyhu.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.hesvh.cn/Article/details/gpeodkull.sHtML

[T27] Swift：错误处理
来源：http://blog.fehbvm.com/Article/details/grralnagk.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.hesvh.cn/Article/details/gbjpslnrl.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gahxtdqwc.sHtML

enum Color { case red, green }
来源：http://www.share.hesvh.cn/Article/details/glclmajtk.sHtML


<!-- 参考信息 -->