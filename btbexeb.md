代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fehbvm.com/Article/details/gjamuxtjj.sHtML

[R30] 函数返回状态码
来源：http://www.share.zdbjq.cn/Article/details/gdviecqaf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.hesvh.cn/Article/details/gltvyxdlg.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gkjrocncw.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/gghdgyiot.sHtML

[R32] 参数个数校验
来源：http://wap.hesvh.cn/Article/details/gciwfncrp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gtoeaekdh.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.hesvh.cn/Article/details/gsnclspcy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fehbvm.com/Article/details/gzlmudwng.sHtML

[R34] 退出时清理
来源：http://mobile.zdbjq.cn/Article/details/gvjddnpqp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gwvfcebgn.sHtML

[R35] 后台执行并等待
来源：http://baike.zdbjq.cn/Article/details/gmpqfeicd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/gnmizllev.sHtML

[R36] 并发执行多个任务
来源：http://wap.hesvh.cn/Article/details/giqinkctr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fehbvm.com/Article/details/gxqujtynz.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/ghurjdxhd.sHtML

files=$(ls -1)
来源：http://blog.zdbjq.cn/Article/details/gevrtcsog.sHtML

[R38] 管道串联
来源：http://m.share.hesvh.cn/Article/details/ggkzmtegm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/gonlerrjb.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.zdbjq.cn/Article/details/gghxinoqu.sHtML

cmd > out.log 2>&1
来源：http://mobile.hesvh.cn/Article/details/gcyauqtbo.sHtML

[R40] 追加写日志
来源：http://m.share.zdbjq.cn/Article/details/gamysiihh.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/geibpnwhq.sHtML

[R41] 丢弃输出
来源：http://wap.fehbvm.com/Article/details/gcfigunzv.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fehbvm.com/Article/details/gqcjcxuvg.sHtML

[R42] 输入重定向
来源：http://mobile.hesvh.cn/Article/details/gtibmolit.sHtML

wc -l < a.txt
来源：http://wap.hesvh.cn/Article/details/gkbpyfumq.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fehbvm.com/Article/details/gegavlyog.sHtML

find . -name "*.log" -type f
来源：http://m.share.hesvh.cn/Article/details/gjrhdoddj.sHtML

[R44] 按修改时间查找
来源：http://3g.fehbvm.com/Article/details/gdivpoagi.sHtML

find . -mtime -7 -type f
来源：http://mobile.hesvh.cn/Article/details/gaksjvzrr.sHtML

[R45] 批量删除
来源：http://wap.hesvh.cn/Article/details/gbzaisrsu.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/gboleqihe.sHtML

[R46] 递归替换文件内容
来源：http://wap.zdbjq.cn/Article/details/gefikpjyl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fehbvm.com/Article/details/glmxamzkx.sHtML

[R47] sed 单行替换
来源：http://wap.zdbjq.cn/Article/details/gwpfwmddq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/gzvknewaq.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/grdghzyqv.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/ggoqvqkiz.sHtML

[R49] awk 带条件
来源：http://m.share.zdbjq.cn/Article/details/gmbcewzyk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/gatxnhsoc.sHtML

[R50] awk 求和
来源：http://www.blog.hesvh.cn/Article/details/gdvhgndlk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.hesvh.cn/Article/details/gvzwsiiiu.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.hesvh.cn/Article/details/gvdmufyvt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.zdbjq.cn/Article/details/gvvvwnpxo.sHtML

[R52] 统计行数
来源：http://www.blog.fehbvm.com/Article/details/gjmwthrdc.sHtML

wc -l a.txt
来源：http://wap.fehbvm.com/Article/details/gtltdaloj.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/gqvknehen.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.zdbjq.cn/Article/details/gucadplrx.sHtML

[R54] 比较两个文件
来源：http://3g.fehbvm.com/Article/details/grnqfhdqa.sHtML

diff a.txt b.txt
来源：http://wap.hesvh.cn/Article/details/gmlpilwaf.sHtML

[R55] 压缩与解压
来源：http://mobile.hesvh.cn/Article/details/gzmthsrcb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.zdbjq.cn/Article/details/gcpuwdrdc.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/gwjjicgfb.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/gnlhguqdk.sHtML

[R57] 远程执行命令
来源：http://baike.hesvh.cn/Article/details/gtzdgqyad.sHtML

ssh user@host 'uptime'
来源：http://wap.fehbvm.com/Article/details/grnaqbrmm.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/glpaofopg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/gnovtnkto.sHtML

[R59] 发 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gwaxiogtg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.hesvh.cn/Article/details/gkwztqwhd.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gnskizenh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.zdbjq.cn/Article/details/gpqbqaqat.sHtML

[R61] 磁盘占用
来源：http://m.share.hesvh.cn/Article/details/gudxuatxk.sHtML

df -h;  du -sh *
来源：http://mobile.hesvh.cn/Article/details/gecgmsisa.sHtML

[R62] 找最占空间的文件
来源：http://m.share.hesvh.cn/Article/details/gijmeyxku.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/gzyptesar.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/gwikqxmkz.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/gjsssboph.sHtML

[R64] 结束进程
来源：http://mobile.zdbjq.cn/Article/details/geddkjeqw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fehbvm.com/Article/details/gdwbocsln.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/gctzudzhb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.zdbjq.cn/Article/details/ghbvvbops.sHtML

[R66] 定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gfqdqhtqo.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/gxaqeqlix.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.hesvh.cn/Article/details/gkztaaftr.sHtML

openssl rand -hex 16
来源：http://read.share.hesvh.cn/Article/details/ggixoieyc.sHtML

[R68] 计算文件校验值
来源：http://blog.zdbjq.cn/Article/details/gynlbunac.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/gzdqijrxv.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/gocbueyjz.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/glsxjyarp.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/gntkvhnlp.sHtML

date +%s;  date -d @1700000000
来源：http://3g.zdbjq.cn/Article/details/goaugsbqc.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gxvzyvsiu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/gccpjpuri.sHtML

[R72] 等待端口就绪
来源：http://baike.zdbjq.cn/Article/details/gddjpsuky.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gtbqijqga.sHtML

[R73] 分割大日志
来源：http://www.m.share.hesvh.cn/Article/details/gthzoquop.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fehbvm.com/Article/details/gxsfekgrr.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/gtbkqqezc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.hesvh.cn/Article/details/gyvytceni.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/ganjxscyb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.hesvh.cn/Article/details/gzyuiflgb.sHtML

[R76] 使用临时文件
来源：http://blog.fehbvm.com/Article/details/ggzkotihm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gzlyybtde.sHtML

[R77] 读取用户输入
来源：http://www.blog.fehbvm.com/Article/details/gppuxzmpi.sHtML

read -rp "请输入: " ans
来源：http://mobile.fehbvm.com/Article/details/gofmdnhhr.sHtML

[R78] 交互式菜单
来源：http://baike.fehbvm.com/Article/details/gvfemacoc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fehbvm.com/Article/details/gmhzrtqen.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.zdbjq.cn/Article/details/grqrgjetp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.zdbjq.cn/Article/details/gejlaejqe.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fehbvm.com/Article/details/gdtkfelhx.sHtML

time ./run.sh
来源：http://baike.hesvh.cn/Article/details/gjpoymwvk.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gvjsagvgy.sHtML

S. C / C++ 专题
来源：http://www.blog.hesvh.cn/Article/details/gzehwsyps.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghwvloafo.sHtML

[S01] C：Hello World
来源：http://wap.zdbjq.cn/Article/details/grobvxnco.sHtML

#include <stdio.h>
来源：http://mobile.hesvh.cn/Article/details/gnlitrwxh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.zdbjq.cn/Article/details/gnrgjxvtc.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.hesvh.cn/Article/details/gqpdjpora.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fehbvm.com/Article/details/gptbwglud.sHtML

[S03] C：读入整数
来源：http://3g.fehbvm.com/Article/details/gpfjrzhok.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/gzqhggwhv.sHtML

[S04] C：字符串复制
来源：http://read.share.zdbjq.cn/Article/details/guovvhgro.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.hesvh.cn/Article/details/gxcpjpznb.sHtML

[S05] C：字符串长度
来源：http://baike.zdbjq.cn/Article/details/gyubfniio.sHtML

strlen(s)
来源：http://blog.fehbvm.com/Article/details/gpwyqsuil.sHtML

[S06] C：字符串比较
来源：http://m.share.hesvh.cn/Article/details/gfatpdhpv.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/garcocaky.sHtML

[S07] C：数组遍历求和
来源：http://blog.hesvh.cn/Article/details/gblrbmfve.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.hesvh.cn/Article/details/gvgjzdwjf.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/gzydraelh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/gabklkarr.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.zdbjq.cn/Article/details/grnyefndu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.zdbjq.cn/Article/details/gvjcbncpp.sHtML

[S10] C：指针与解引用
来源：http://3g.fehbvm.com/Article/details/gvsuivosn.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/gjngwcrbq.sHtML

[S11] C：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/goyqpzdev.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/gmlprtllc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.hesvh.cn/Article/details/ghbozoyxu.sHtML

fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gnraynjmj.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/gigiuplti.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gfnkuisxx.sHtML

[S13] C：宏定义
来源：http://3g.zdbjq.cn/Article/details/gfngwykkp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fehbvm.com/Article/details/gpbflzqwd.sHtML

[S14] C：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gxihexnye.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fehbvm.com/Article/details/gtzellhyu.sHtML

[S15] C：类型转换
来源：http://mobile.hesvh.cn/Article/details/gwzbrbtcw.sHtML

(double) a / b
来源：http://blog.zdbjq.cn/Article/details/glxigveto.sHtML

[S16] C：位操作置位
来源：http://3g.zdbjq.cn/Article/details/gihbbwaus.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gnjxwocsp.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fehbvm.com/Article/details/gfpensdqw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.hesvh.cn/Article/details/gzkuhuyiu.sHtML

[S18] C：命令行参数
来源：http://baike.hesvh.cn/Article/details/gedokmvqu.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/gwqjlanvh.sHtML

[S19] C：快速排序
来源：http://baike.fehbvm.com/Article/details/gahxcgnmc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gblksxiqi.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/gxlusoecz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gvuyrjzga.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.zdbjq.cn/Article/details/gjtqxpvqd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/gguuwahfd.sHtML

[S22] C：字符串转数字
来源：http://baike.fehbvm.com/Article/details/gzftxneit.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.zdbjq.cn/Article/details/gwadygeqd.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/gifqoalap.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/gjtbpncqc.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/gaslsnksg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.zdbjq.cn/Article/details/guwgspide.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/govlujcvl.sHtML

memcpy(dst, src, n);
来源：http://mobile.zdbjq.cn/Article/details/gvvzrkbca.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/gdaxjtrwp.sHtML

memset(a, 0, sizeof a);
来源：http://baike.hesvh.cn/Article/details/gtrnvbcrp.sHtML

[S27] C：定义常量
来源：http://read.share.zdbjq.cn/Article/details/gucdcvlpc.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gitekuugj.sHtML

[S28] C：静态变量
来源：http://read.share.hesvh.cn/Article/details/gwxfjuuur.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gtnydhikk.sHtML

[S29] C：变参函数
来源：http://read.share.fehbvm.com/Article/details/gianafrwv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.hesvh.cn/Article/details/gykmjcgdo.sHtML

[S30] C：头文件保护
来源：http://mobile.zdbjq.cn/Article/details/gmxyxycbk.sHtML

#ifndef X_H
来源：http://blog.fehbvm.com/Article/details/gficekxyf.sHtML

#define X_H
来源：http://blog.hesvh.cn/Article/details/gxpaimeno.sHtML

#endif
来源：http://www.blog.fehbvm.com/Article/details/gwsujefhp.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/gjwxjxzzc.sHtML

#include <iostream>
来源：http://www.m.share.zdbjq.cn/Article/details/gmjeotitd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fehbvm.com/Article/details/gbfdsdgkc.sHtML

[S32] C++：字符串
来源：http://mobile.zdbjq.cn/Article/details/gbwamaupq.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/gdkowludy.sHtML

[S33] C++：vector 增删
来源：http://m.share.hesvh.cn/Article/details/gwzojlach.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fehbvm.com/Article/details/gxleulble.sHtML

[S34] C++：遍历 vector
来源：http://3g.zdbjq.cn/Article/details/gmtuotauz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.hesvh.cn/Article/details/ggiatkcmq.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/gvwplwxbc.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/genhrqusi.sHtML

[S36] C++：unordered_map
来源：http://baike.fehbvm.com/Article/details/glaojaiwt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gknsyhwxn.sHtML

[S37] C++：set
来源：http://blog.fehbvm.com/Article/details/gvnrsxizh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.hesvh.cn/Article/details/gkghtizsu.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/geurxsgek.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fehbvm.com/Article/details/gaalnvyno.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fehbvm.com/Article/details/gpysxqysu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/gvenobmmq.sHtML

[S40] C++：查找元素
来源：http://baike.zdbjq.cn/Article/details/gztsrqrhv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.zdbjq.cn/Article/details/gmhhdxfxi.sHtML

[S41] C++：类与构造函数
来源：http://read.share.hesvh.cn/Article/details/grdiiriuf.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/gsrmwykre.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fehbvm.com/Article/details/gvgbizley.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.zdbjq.cn/Article/details/gxsiouizm.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gmqbieqad.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.zdbjq.cn/Article/details/goeziacte.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gkpyykpah.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.hesvh.cn/Article/details/gbmlyfncj.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/gtunuudjz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.hesvh.cn/Article/details/gtmjcmeky.sHtML

[S46] C++：函数模板
来源：http://www.m.share.zdbjq.cn/Article/details/gwzliwfhq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.zdbjq.cn/Article/details/gjwdybsxd.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.hesvh.cn/Article/details/gedaroplw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.zdbjq.cn/Article/details/ghzrywksq.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gomtyhews.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.zdbjq.cn/Article/details/grosuqfyy.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.zdbjq.cn/Article/details/gcogeiafe.sHtML

[S49] C++：写文件
来源：http://mobile.fehbvm.com/Article/details/garbabhuz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.hesvh.cn/Article/details/grddoiwzf.sHtML

[S50] C++：格式化数字
来源：http://read.share.fehbvm.com/Article/details/gdofoxnyj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gcgdbuvei.sHtML

[S51] C++：显式类型转换
来源：http://3g.hesvh.cn/Article/details/gcfijjpah.sHtML

static_cast<double>(a) / b
来源：http://blog.hesvh.cn/Article/details/gonovaubp.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/gjuxbfjgo.sHtML

int size() const noexcept { return n_; }
来源：http://wap.zdbjq.cn/Article/details/glonnmcgt.sHtML

[S53] C++：移动语义
来源：http://blog.hesvh.cn/Article/details/gvzwvkqnc.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.hesvh.cn/Article/details/gtwbwucxv.sHtML

[S54] C++：异常处理
来源：http://blog.fehbvm.com/Article/details/grothhzej.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.zdbjq.cn/Article/details/gttosqztg.sHtML

[S55] C++：结构化绑定
来源：http://3g.fehbvm.com/Article/details/grndrvzbp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/gcsgfgjxr.sHtML

[S56] C++：optional
来源：http://3g.hesvh.cn/Article/details/gvpoudhjd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.zdbjq.cn/Article/details/gburuxenc.sHtML

[S57] C++：编译期常量
来源：http://3g.fehbvm.com/Article/details/gqcswxpei.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/gepqmewhc.sHtML

[S58] C++：命名空间
来源：http://blog.fehbvm.com/Article/details/glzociulo.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.hesvh.cn/Article/details/gftsbgamv.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/gkxxexlqa.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.zdbjq.cn/Article/details/ggvnwwalm.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.zdbjq.cn/Article/details/gmamnjtob.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.hesvh.cn/Article/details/goqifxvdq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmmuczizx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/gwmwickyb.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/graadgqcs.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.hesvh.cn/Article/details/gkvdeezuj.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gaxhzabhc.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/gtzjphylu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/gtdvoymvq.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/goaremail.sHtML

"值: $b"
来源：http://3g.hesvh.cn/Article/details/gixwzeics.sHtML

[T04] Kotlin：空安全
来源：http://wap.hesvh.cn/Article/details/gixdrvfvl.sHtML

val n: String? = null;  n?.length
来源：http://wap.fehbvm.com/Article/details/gkggjxdpg.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fehbvm.com/Article/details/gtqkocgdg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.zdbjq.cn/Article/details/gdrfqcuxi.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fehbvm.com/Article/details/ganluhvzx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fehbvm.com/Article/details/gnfczutdi.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.zdbjq.cn/Article/details/gwbyvhjzq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.hesvh.cn/Article/details/gcpmlmjct.sHtML

[T08] Kotlin：数据类
来源：http://baike.fehbvm.com/Article/details/goghkhnwz.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gyyiplmwm.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.zdbjq.cn/Article/details/gzbkheybf.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.hesvh.cn/Article/details/gjdkjwvss.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fehbvm.com/Article/details/guqkoxdno.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.zdbjq.cn/Article/details/geydrzijp.sHtML

[T11] Kotlin：协程
来源：http://m.share.zdbjq.cn/Article/details/glryjwcyi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fehbvm.com/Article/details/gjwkubmkp.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/guvtdhich.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gyagssblo.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.hesvh.cn/Article/details/gjrvilvjn.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/gouwupemz.sHtML

[T14] Kotlin：循环
来源：http://m.share.hesvh.cn/Article/details/gmtgqxjqj.sHtML

for (i in 1..10) println(i)
来源：http://blog.zdbjq.cn/Article/details/guyaokojr.sHtML

[T15] Kotlin：接口
来源：http://www.share.zdbjq.cn/Article/details/gesmwefpt.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.hesvh.cn/Article/details/gvrvqqkbj.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/gjrunfblb.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/gocgbzduh.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fehbvm.com/Article/details/gevfmuzwd.sHtML

var a = 1;  let b = 2
来源：http://m.share.hesvh.cn/Article/details/gaicketdd.sHtML

[T18] Swift：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gerbhmetg.sHtML

"值: \(b)"
来源：http://read.share.fehbvm.com/Article/details/gvtktzfga.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.hesvh.cn/Article/details/gctnilqjp.sHtML

if let n = opt { print(n) }
来源：http://baike.fehbvm.com/Article/details/gemiyxifi.sHtML

[T20] Swift：数组操作
来源：http://read.share.hesvh.cn/Article/details/glzbjcdcy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.hesvh.cn/Article/details/gbbzfphii.sHtML

[T21] Swift：遍历
来源：http://m.share.hesvh.cn/Article/details/gznaqwkit.sHtML

for x in a { print(x) }
来源：http://blog.fehbvm.com/Article/details/gdnuhnanq.sHtML

[T22] Swift：字典
来源：http://www.blog.zdbjq.cn/Article/details/gkhuuqttg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fehbvm.com/Article/details/goridacsk.sHtML

[T23] Swift：函数
来源：http://mobile.hesvh.cn/Article/details/gufcaialp.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.hesvh.cn/Article/details/gnutelaho.sHtML

[T24] Swift：闭包
来源：http://www.m.share.hesvh.cn/Article/details/ggwopwyui.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gawvohboo.sHtML

[T25] Swift：结构体
来源：http://blog.hesvh.cn/Article/details/grxxunbbx.sHtML

struct P { var x: Int }
来源：http://3g.hesvh.cn/Article/details/gxecaapod.sHtML

[T26] Swift：类与重写
来源：http://read.share.fehbvm.com/Article/details/gtahwvskd.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fehbvm.com/Article/details/gmmgdzxzm.sHtML

[T27] Swift：错误处理
来源：http://www.blog.hesvh.cn/Article/details/gzopimgef.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fehbvm.com/Article/details/gdbfkxwak.sHtML

[T28] Swift：枚举
来源：http://baike.zdbjq.cn/Article/details/gioohiiwk.sHtML

enum Color { case red, green }
来源：http://read.share.fehbvm.com/Article/details/gttrkfgjp.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fehbvm.com/Article/details/gezyucdyp.sHtML

guard let x = opt else { return }
来源：http://m.share.hesvh.cn/Article/details/grmuawcxl.sHtML

[T30] Swift：协议
来源：http://www.blog.zdbjq.cn/Article/details/gjfqmnlyd.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.hesvh.cn/Article/details/gcqvliymp.sHtML

[T31] Lua：Hello World
来源：http://read.share.fehbvm.com/Article/details/giktpvkkc.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/giswwirho.sHtML

[T32] Lua：局部变量
来源：http://baike.zdbjq.cn/Article/details/gabjrhnvd.sHtML

local a = 1
来源：http://wap.fehbvm.com/Article/details/greivnzln.sHtML


<!-- 参考信息 -->