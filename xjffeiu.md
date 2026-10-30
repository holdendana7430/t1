代发 wailian999

echo $((1 + 2 * 3))
来源：http://baike.fehbvm.com/Article/details/guuglixyo.sHtML

[R28] 浮点运算
来源：http://3g.zdbjq.cn/Article/details/gukurzipo.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fehbvm.com/Article/details/gocddclmf.sHtML

[R29] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gtatalbhd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.hesvh.cn/Article/details/gqcvetgrd.sHtML

[R30] 函数返回状态码
来源：http://www.blog.zdbjq.cn/Article/details/gztreaxyb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.zdbjq.cn/Article/details/grfbvhzbv.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/gatrfsvmr.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fehbvm.com/Article/details/glvgheceo.sHtML

[R32] 参数个数校验
来源：http://baike.zdbjq.cn/Article/details/gokfpxuod.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/ghxmqqzcj.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.zdbjq.cn/Article/details/gfkcdnson.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/gdfynurte.sHtML

[R34] 退出时清理
来源：http://baike.zdbjq.cn/Article/details/gijfyhpcr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/ghqhtoonc.sHtML

[R35] 后台执行并等待
来源：http://blog.fehbvm.com/Article/details/gjwwtidcn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.hesvh.cn/Article/details/gcxmerzus.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/gaqrhlxsg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fehbvm.com/Article/details/gtmsqnixe.sHtML

[R37] 把输出赋给变量
来源：http://mobile.zdbjq.cn/Article/details/gcpmsshxj.sHtML

files=$(ls -1)
来源：http://blog.zdbjq.cn/Article/details/gidrojlgl.sHtML

[R38] 管道串联
来源：http://mobile.hesvh.cn/Article/details/gjzaodbxn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.hesvh.cn/Article/details/ggdoewjbx.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/gjzfxleqw.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/gnnitloir.sHtML

[R40] 追加写日志
来源：http://www.share.hesvh.cn/Article/details/gracccocv.sHtML

echo "log" >> out.log
来源：http://www.m.share.fehbvm.com/Article/details/gznotkxwo.sHtML

[R41] 丢弃输出
来源：http://www.blog.fehbvm.com/Article/details/ggrdpsoeq.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fehbvm.com/Article/details/gzpqdaogo.sHtML

[R42] 输入重定向
来源：http://www.share.fehbvm.com/Article/details/ggapjiqhk.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gjpynwmad.sHtML

[R43] 按名字查找文件
来源：http://m.share.zdbjq.cn/Article/details/gdsrnsaev.sHtML

find . -name "*.log" -type f
来源：http://www.share.fehbvm.com/Article/details/gzpbafbrx.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/gghhrdhsh.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fehbvm.com/Article/details/ggiisfeky.sHtML

[R45] 批量删除
来源：http://blog.hesvh.cn/Article/details/gboqmenlz.sHtML

find . -name "*.tmp" -delete
来源：http://3g.zdbjq.cn/Article/details/gxbbpnhty.sHtML

[R46] 递归替换文件内容
来源：http://blog.hesvh.cn/Article/details/goivtjqre.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fehbvm.com/Article/details/grykskjem.sHtML

[R47] sed 单行替换
来源：http://wap.fehbvm.com/Article/details/gcplxszpj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.hesvh.cn/Article/details/gmlnycxca.sHtML

[R48] awk 取指定列
来源：http://wap.hesvh.cn/Article/details/gwbziddzs.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gsgpomhps.sHtML

[R49] awk 带条件
来源：http://www.m.share.hesvh.cn/Article/details/gblyrbyri.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.zdbjq.cn/Article/details/gbkqfnabw.sHtML

[R50] awk 求和
来源：http://www.blog.zdbjq.cn/Article/details/gmhedhopl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/grumeosvd.sHtML

[R51] 排序去重取前几
来源：http://www.share.zdbjq.cn/Article/details/gspojyasf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/ghtjxsurt.sHtML

[R52] 统计行数
来源：http://baike.hesvh.cn/Article/details/gptbkffub.sHtML

wc -l a.txt
来源：http://www.blog.fehbvm.com/Article/details/glwebhvta.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.hesvh.cn/Article/details/guzttnjfn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.zdbjq.cn/Article/details/gucaaklpg.sHtML

[R54] 比较两个文件
来源：http://m.share.hesvh.cn/Article/details/gdmsakwhu.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/gepvkxxbu.sHtML

[R55] 压缩与解压
来源：http://read.share.zdbjq.cn/Article/details/gzrlimgzt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.hesvh.cn/Article/details/gculknazb.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/gmwmfucfu.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/gegfnfdpn.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fehbvm.com/Article/details/gqegvypcr.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fehbvm.com/Article/details/gtrcqzwif.sHtML

[R58] 下载文件
来源：http://blog.hesvh.cn/Article/details/gyauslccl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.hesvh.cn/Article/details/gmvwyttgf.sHtML

[R59] 发 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gksnsmsci.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fehbvm.com/Article/details/gmgwwvece.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gtbfkusks.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fehbvm.com/Article/details/gebysuvcr.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/gdqmeupob.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/grpmaoakf.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/gdprxmslo.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gsckxlbil.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/glxmepjkp.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.hesvh.cn/Article/details/gvudivvbk.sHtML

[R64] 结束进程
来源：http://blog.hesvh.cn/Article/details/gumorfskf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.hesvh.cn/Article/details/gcunofgzs.sHtML

[R65] 查看端口占用
来源：http://m.share.fehbvm.com/Article/details/ggvufcykb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.zdbjq.cn/Article/details/glfemoydp.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/gdrobncbf.sHtML

crontab -e;  crontab -l
来源：http://m.share.hesvh.cn/Article/details/gblglavvs.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/gqamuvbkt.sHtML

openssl rand -hex 16
来源：http://3g.zdbjq.cn/Article/details/gtpnuypzx.sHtML

[R68] 计算文件校验值
来源：http://wap.hesvh.cn/Article/details/gdmoxokop.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.hesvh.cn/Article/details/gueoueqel.sHtML

[R69] 生成随机密码
来源：http://read.share.hesvh.cn/Article/details/gexeugmng.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.zdbjq.cn/Article/details/gycapfkcx.sHtML

[R70] 时间戳与互转
来源：http://wap.zdbjq.cn/Article/details/gjrnanjgk.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fehbvm.com/Article/details/gwfkpfpit.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/grfwtsagl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.zdbjq.cn/Article/details/gsmynjize.sHtML

[R72] 等待端口就绪
来源：http://blog.hesvh.cn/Article/details/gmdrgdxvr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gbbudpnnt.sHtML

[R73] 分割大日志
来源：http://wap.fehbvm.com/Article/details/gwjhsmuiz.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/gesvzrtzy.sHtML

[R74] 批量重命名
来源：http://www.m.share.zdbjq.cn/Article/details/gjfqoztdc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.hesvh.cn/Article/details/gigjbkbay.sHtML

[R75] 导出环境变量
来源：http://www.share.hesvh.cn/Article/details/gtqtopoju.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fehbvm.com/Article/details/glvrwmgow.sHtML

[R76] 使用临时文件
来源：http://www.blog.hesvh.cn/Article/details/ggvonheps.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gshidrunc.sHtML

[R77] 读取用户输入
来源：http://www.share.hesvh.cn/Article/details/gzmpwbeyr.sHtML

read -rp "请输入: " ans
来源：http://wap.fehbvm.com/Article/details/gntcmihtn.sHtML

[R78] 交互式菜单
来源：http://www.share.fehbvm.com/Article/details/gjpeknvhi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fehbvm.com/Article/details/gpkeauapv.sHtML

[R79] 解析命令行选项
来源：http://m.share.fehbvm.com/Article/details/ghydiygmt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fehbvm.com/Article/details/giyabohnj.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.hesvh.cn/Article/details/gwnnrznbp.sHtML

time ./run.sh
来源：http://3g.zdbjq.cn/Article/details/gmkxliqgp.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjlbetlam.sHtML

S. C / C++ 专题
来源：http://3g.hesvh.cn/Article/details/ghaojglda.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gofiwlpfe.sHtML

[S01] C：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/ghquhnmzx.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/giuvwksee.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.hesvh.cn/Article/details/gtifaaoum.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.hesvh.cn/Article/details/guwjwexgm.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.hesvh.cn/Article/details/gfztwnlvc.sHtML

[S03] C：读入整数
来源：http://baike.zdbjq.cn/Article/details/ggprwbexn.sHtML

int x; scanf("%d", &x);
来源：http://wap.fehbvm.com/Article/details/goxvitydo.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/guoqnflyi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/goektutep.sHtML

[S05] C：字符串长度
来源：http://3g.fehbvm.com/Article/details/grefvhepr.sHtML

strlen(s)
来源：http://blog.fehbvm.com/Article/details/gxyshshfj.sHtML

[S06] C：字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gfpgyhcyu.sHtML

strcmp(a, b) == 0
来源：http://baike.fehbvm.com/Article/details/gaxeelmnk.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/gtbtpjedf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.hesvh.cn/Article/details/gbwopsltp.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.hesvh.cn/Article/details/gahxkxtni.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fehbvm.com/Article/details/gmvurtxvb.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/gwdngalgd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/gwzbsndro.sHtML

[S10] C：指针与解引用
来源：http://www.share.fehbvm.com/Article/details/gxcruwiwf.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fehbvm.com/Article/details/gvkfuaofh.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gmntduwyt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.zdbjq.cn/Article/details/gidlmwjlt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/gxynvdrxl.sHtML

fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gxdugftyr.sHtML

[S12] C：写文件
来源：http://baike.zdbjq.cn/Article/details/gqnavheee.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.hesvh.cn/Article/details/gnlesiyve.sHtML

[S13] C：宏定义
来源：http://www.m.share.fehbvm.com/Article/details/giyqksvyf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/gwgawppwn.sHtML

[S14] C：枚举
来源：http://www.blog.fehbvm.com/Article/details/gtjkmeiii.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.hesvh.cn/Article/details/ggwilxqny.sHtML

[S15] C：类型转换
来源：http://www.blog.hesvh.cn/Article/details/gyrggpgta.sHtML

(double) a / b
来源：http://blog.zdbjq.cn/Article/details/gqzbslrot.sHtML

[S16] C：位操作置位
来源：http://baike.hesvh.cn/Article/details/gumncufjc.sHtML

x |= (1 << 3);
来源：http://wap.zdbjq.cn/Article/details/gjfqzylcu.sHtML

[S17] C：安全拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gxcrcwqlm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/gevhsiohy.sHtML

[S18] C：命令行参数
来源：http://www.share.zdbjq.cn/Article/details/glmmigqlp.sHtML

int main(int argc, char **argv)
来源：http://3g.zdbjq.cn/Article/details/grmstxzoa.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/gicixuead.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gdpavwsdb.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/gxbmxirau.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gxwvwqksz.sHtML

[S21] C：字符类别判断
来源：http://www.blog.zdbjq.cn/Article/details/goeaolknw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.hesvh.cn/Article/details/gwhpwslyp.sHtML

[S22] C：字符串转数字
来源：http://mobile.hesvh.cn/Article/details/ggujeaxyr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.hesvh.cn/Article/details/gzhaqzoda.sHtML

[S23] C：随机数
来源：http://mobile.fehbvm.com/Article/details/ghyqnxbfq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/guzwhekej.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/gylxlfsbn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/gxjpvuutw.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/gncvsmvoe.sHtML

memcpy(dst, src, n);
来源：http://3g.fehbvm.com/Article/details/gyniddyxm.sHtML

[S26] C：内存清零
来源：http://baike.zdbjq.cn/Article/details/gkokpklnw.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/gfxqgorri.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/gmtxtznph.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gpdjgilyf.sHtML

[S28] C：静态变量
来源：http://blog.hesvh.cn/Article/details/gzfpeyczi.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/giphefkqz.sHtML

[S29] C：变参函数
来源：http://www.blog.zdbjq.cn/Article/details/ggjvushhf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.hesvh.cn/Article/details/gboxflfpu.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/gvoneogaq.sHtML

#ifndef X_H
来源：http://baike.zdbjq.cn/Article/details/ghkphkrzw.sHtML

#define X_H
来源：http://3g.hesvh.cn/Article/details/gzdewrpyz.sHtML

#endif
来源：http://www.m.share.fehbvm.com/Article/details/gxqdrmrnn.sHtML

[S31] C++：Hello World
来源：http://baike.zdbjq.cn/Article/details/gscznzojq.sHtML

#include <iostream>
来源：http://baike.hesvh.cn/Article/details/gzhznhxvm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.hesvh.cn/Article/details/gdbowktfy.sHtML

[S32] C++：字符串
来源：http://m.share.fehbvm.com/Article/details/gvjhjlcwc.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/gkxxbnxvj.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/gbegcnwwh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fehbvm.com/Article/details/gatjamiti.sHtML

[S34] C++：遍历 vector
来源：http://baike.zdbjq.cn/Article/details/ghmesmgjb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fehbvm.com/Article/details/guoejcmls.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/gyedhhoss.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gwiiscxeo.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/gxnptezar.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gmqnlczjb.sHtML

[S37] C++：set
来源：http://m.share.zdbjq.cn/Article/details/gcamfhygu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/gfetldrcb.sHtML

[S38] C++：排序
来源：http://baike.zdbjq.cn/Article/details/gbtcbjieb.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.hesvh.cn/Article/details/gwdtdffrn.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.zdbjq.cn/Article/details/goditzezw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.hesvh.cn/Article/details/gmyjtzfzm.sHtML

[S40] C++：查找元素
来源：http://wap.fehbvm.com/Article/details/goyniqovj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.zdbjq.cn/Article/details/gzliopyqh.sHtML

[S41] C++：类与构造函数
来源：http://m.share.zdbjq.cn/Article/details/gubdikmbq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/gljbmmidq.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.zdbjq.cn/Article/details/gduqejlft.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.zdbjq.cn/Article/details/gzwkutngt.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/gonjipefv.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.hesvh.cn/Article/details/ghnukhqgd.sHtML

[S44] C++：引用传参
来源：http://3g.fehbvm.com/Article/details/gjzjxeris.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.zdbjq.cn/Article/details/gyvctzowj.sHtML

[S45] C++：lambda
来源：http://blog.hesvh.cn/Article/details/gvtgdpdtp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/gmkbdciox.sHtML

[S46] C++：函数模板
来源：http://www.share.hesvh.cn/Article/details/ginvzwqif.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.hesvh.cn/Article/details/giqabsfat.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.zdbjq.cn/Article/details/gzbgvxjtz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fehbvm.com/Article/details/gekfbsbgb.sHtML

[S48] C++：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gwdcgzees.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/gxowfhmsy.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fehbvm.com/Article/details/ggqoqvzev.sHtML

[S49] C++：写文件
来源：http://m.share.fehbvm.com/Article/details/gtmxfvmll.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.hesvh.cn/Article/details/gfljggqan.sHtML

[S50] C++：格式化数字
来源：http://wap.hesvh.cn/Article/details/gjtzizkgb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gllsrlmhw.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gzmqikuje.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gbxrumapa.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fehbvm.com/Article/details/gtkfidueg.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.hesvh.cn/Article/details/giimohvrc.sHtML

[S53] C++：移动语义
来源：http://read.share.fehbvm.com/Article/details/gzurcsyss.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/gizurdniz.sHtML

[S54] C++：异常处理
来源：http://baike.fehbvm.com/Article/details/grkfxmfgq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.zdbjq.cn/Article/details/gayjqgivj.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fehbvm.com/Article/details/gcibfrzdi.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/gpxgmigjl.sHtML

[S56] C++：optional
来源：http://wap.fehbvm.com/Article/details/grxxojqfg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/gzykhombw.sHtML

[S57] C++：编译期常量
来源：http://blog.hesvh.cn/Article/details/geudrojyn.sHtML

constexpr int N = 10;
来源：http://blog.zdbjq.cn/Article/details/glxnplsvh.sHtML

[S58] C++：命名空间
来源：http://www.share.hesvh.cn/Article/details/ggwillehn.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.hesvh.cn/Article/details/gkxbzvcce.sHtML

[S59] C++：静态断言
来源：http://baike.zdbjq.cn/Article/details/ggzpchdes.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fehbvm.com/Article/details/gyzevdyms.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fehbvm.com/Article/details/glnwfehtd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.hesvh.cn/Article/details/ghqwblgqu.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkantryaz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/ggxwpqudb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnqynsbik.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gbeajbzuo.sHtML

println("Hello")
来源：http://read.share.fehbvm.com/Article/details/gpwxfycul.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/gsoeubpje.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/gciufnecf.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.hesvh.cn/Article/details/guqmqxzvx.sHtML

"值: $b"
来源：http://read.share.hesvh.cn/Article/details/gjmlfarko.sHtML

[T04] Kotlin：空安全
来源：http://wap.fehbvm.com/Article/details/gdvsklpix.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.hesvh.cn/Article/details/gnnoebkkm.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.zdbjq.cn/Article/details/gbotroerl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.zdbjq.cn/Article/details/gmpvpdsgb.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gjnbgdveg.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/gumluwghd.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.zdbjq.cn/Article/details/gtpfayzig.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fehbvm.com/Article/details/gohlankrq.sHtML

[T08] Kotlin：数据类
来源：http://wap.hesvh.cn/Article/details/grbpynpoq.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/ghflgsaug.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/gmyljubnu.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.zdbjq.cn/Article/details/gaqqpmpbo.sHtML

[T10] Kotlin：默认参数
来源：http://blog.hesvh.cn/Article/details/gwhgcslvs.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.zdbjq.cn/Article/details/garbhfinw.sHtML

[T11] Kotlin：协程
来源：http://wap.zdbjq.cn/Article/details/goaxyfbbw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.fehbvm.com/Article/details/gghphvndr.sHtML

[T12] Kotlin：解构声明
来源：http://3g.zdbjq.cn/Article/details/gaxetfwtu.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gssxvvymt.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.hesvh.cn/Article/details/gmnefexmu.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fehbvm.com/Article/details/ghoeomcrx.sHtML

[T14] Kotlin：循环
来源：http://3g.fehbvm.com/Article/details/gjtvzzsow.sHtML

for (i in 1..10) println(i)
来源：http://baike.hesvh.cn/Article/details/ggobccnsr.sHtML

[T15] Kotlin：接口
来源：http://www.blog.hesvh.cn/Article/details/gehhljfim.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fehbvm.com/Article/details/gfwvyszxz.sHtML

[T16] Swift：Hello World
来源：http://www.share.hesvh.cn/Article/details/gvhplycap.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gdorfchqg.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fehbvm.com/Article/details/gvqlkrbvg.sHtML

var a = 1;  let b = 2
来源：http://m.share.hesvh.cn/Article/details/gsyogkvmf.sHtML

[T18] Swift：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gzmhqbmbv.sHtML

"值: \(b)"
来源：http://m.share.hesvh.cn/Article/details/ggftlewjb.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gaeximhbq.sHtML

if let n = opt { print(n) }
来源：http://mobile.fehbvm.com/Article/details/gjjdyqlfg.sHtML

[T20] Swift：数组操作
来源：http://baike.hesvh.cn/Article/details/gzzfystnz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fehbvm.com/Article/details/glozntvkv.sHtML

[T21] Swift：遍历
来源：http://blog.hesvh.cn/Article/details/guuviajdi.sHtML

for x in a { print(x) }
来源：http://3g.fehbvm.com/Article/details/ggoxprlby.sHtML

[T22] Swift：字典
来源：http://baike.fehbvm.com/Article/details/gtnbdtlht.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/gecwltxor.sHtML

[T23] Swift：函数
来源：http://blog.fehbvm.com/Article/details/gktoqflvh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.hesvh.cn/Article/details/ghuywcuaj.sHtML

[T24] Swift：闭包
来源：http://blog.zdbjq.cn/Article/details/gricrwvwv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.hesvh.cn/Article/details/ghxnhmgmy.sHtML

[T25] Swift：结构体
来源：http://www.blog.hesvh.cn/Article/details/guxftmrdr.sHtML

struct P { var x: Int }
来源：http://www.share.zdbjq.cn/Article/details/ggixdwkmt.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fehbvm.com/Article/details/gxsigdgtc.sHtML

class A: Base { override func f() {} }
来源：http://wap.zdbjq.cn/Article/details/gsevvmyui.sHtML

[T27] Swift：错误处理
来源：http://mobile.zdbjq.cn/Article/details/gvtigpric.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.zdbjq.cn/Article/details/gmilywzhx.sHtML

[T28] Swift：枚举
来源：http://mobile.zdbjq.cn/Article/details/gmodwyxkh.sHtML

enum Color { case red, green }
来源：http://baike.zdbjq.cn/Article/details/gfkcuvblz.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fehbvm.com/Article/details/gmkwvyyin.sHtML

guard let x = opt else { return }
来源：http://baike.zdbjq.cn/Article/details/gaqswdbui.sHtML

[T30] Swift：协议
来源：http://read.share.zdbjq.cn/Article/details/gliydyfcf.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.hesvh.cn/Article/details/gfzjqlcbk.sHtML


<!-- 参考信息 -->