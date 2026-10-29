代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.zdbjq.cn/Article/details/ggpcmfied.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gltywyjjq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/gvvnhmcmw.sHtML

[R31] 局部变量
来源：http://baike.hesvh.cn/Article/details/gxvmttfbf.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/ggbmpiuzo.sHtML

[R32] 参数个数校验
来源：http://read.share.hesvh.cn/Article/details/gomtperrw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gpurbjjkr.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.hesvh.cn/Article/details/gcpzgbsdj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.hesvh.cn/Article/details/ggvcanabz.sHtML

[R34] 退出时清理
来源：http://m.share.zdbjq.cn/Article/details/gkbkzsrzp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/griujgbfs.sHtML

[R35] 后台执行并等待
来源：http://baike.zdbjq.cn/Article/details/grbjtyetr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/gvmlutsdk.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gixzuvhas.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/glcdwpmsk.sHtML

[R37] 把输出赋给变量
来源：http://read.share.hesvh.cn/Article/details/ggyszjdkx.sHtML

files=$(ls -1)
来源：http://baike.hesvh.cn/Article/details/gwihzlnvd.sHtML

[R38] 管道串联
来源：http://www.m.share.hesvh.cn/Article/details/gqlvbmrad.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.zdbjq.cn/Article/details/gizfyqmky.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/gktkllaww.sHtML

cmd > out.log 2>&1
来源：http://blog.hesvh.cn/Article/details/ghgzpcbgc.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/gskzvcvso.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/gfritpwdv.sHtML

[R41] 丢弃输出
来源：http://baike.fehbvm.com/Article/details/gnagohyle.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fehbvm.com/Article/details/ggximpahq.sHtML

[R42] 输入重定向
来源：http://m.share.fehbvm.com/Article/details/ghxoettfo.sHtML

wc -l < a.txt
来源：http://read.share.zdbjq.cn/Article/details/gwhcrkltw.sHtML

[R43] 按名字查找文件
来源：http://m.share.hesvh.cn/Article/details/geczgsnll.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fehbvm.com/Article/details/gttneiyjy.sHtML

[R44] 按修改时间查找
来源：http://mobile.zdbjq.cn/Article/details/gzmrihvqx.sHtML

find . -mtime -7 -type f
来源：http://baike.fehbvm.com/Article/details/ghupbavpi.sHtML

[R45] 批量删除
来源：http://blog.zdbjq.cn/Article/details/gszvvvgtb.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fehbvm.com/Article/details/gufqtosuc.sHtML

[R46] 递归替换文件内容
来源：http://blog.hesvh.cn/Article/details/giudlllzk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gieohcdxp.sHtML

[R47] sed 单行替换
来源：http://wap.zdbjq.cn/Article/details/gixnqfuiw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.zdbjq.cn/Article/details/gkpazyzce.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/gobojncvi.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.hesvh.cn/Article/details/gjtoexgid.sHtML

[R49] awk 带条件
来源：http://wap.zdbjq.cn/Article/details/gqppyizuz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.hesvh.cn/Article/details/gboteykjv.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/gteazuxbf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gqdzvplbl.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/gxfwjfwan.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fehbvm.com/Article/details/gwoqnwvgg.sHtML

[R52] 统计行数
来源：http://blog.hesvh.cn/Article/details/gylqzmvlj.sHtML

wc -l a.txt
来源：http://3g.fehbvm.com/Article/details/gdqazekje.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.zdbjq.cn/Article/details/gmscnfnvg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/gyvskmsjr.sHtML

[R54] 比较两个文件
来源：http://mobile.hesvh.cn/Article/details/ggxudqcud.sHtML

diff a.txt b.txt
来源：http://www.m.share.fehbvm.com/Article/details/gncagedrc.sHtML

[R55] 压缩与解压
来源：http://m.share.zdbjq.cn/Article/details/gkkzbwvum.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/gykxcimxw.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/gsvblunpw.sHtML

scp file user@host:/path/
来源：http://www.share.hesvh.cn/Article/details/gvnxjnuct.sHtML

[R57] 远程执行命令
来源：http://baike.zdbjq.cn/Article/details/gcvfwlmls.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fehbvm.com/Article/details/gnbxfwzrj.sHtML

[R58] 下载文件
来源：http://baike.hesvh.cn/Article/details/gdudkgrsn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.hesvh.cn/Article/details/gafpmmbtq.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gakgqfldv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/gqjqcxhxz.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gygetkuex.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.zdbjq.cn/Article/details/gzpscnnob.sHtML

[R61] 磁盘占用
来源：http://mobile.zdbjq.cn/Article/details/gnyucnznt.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/gdxiefkaw.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/gbnujyvvr.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.hesvh.cn/Article/details/gdwuqurtx.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/gcemfbprm.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.zdbjq.cn/Article/details/gmkhtands.sHtML

[R64] 结束进程
来源：http://3g.hesvh.cn/Article/details/gkhonwako.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.hesvh.cn/Article/details/gdwsidfft.sHtML

[R65] 查看端口占用
来源：http://read.share.hesvh.cn/Article/details/ggugrrkmf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fehbvm.com/Article/details/gjhvfpinf.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/gvufedpza.sHtML

crontab -e;  crontab -l
来源：http://mobile.hesvh.cn/Article/details/gzvzxsvsb.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/gkuzdmbea.sHtML

openssl rand -hex 16
来源：http://wap.fehbvm.com/Article/details/gajhxjsky.sHtML

[R68] 计算文件校验值
来源：http://blog.hesvh.cn/Article/details/gyfpfeefu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gbxfqlvmj.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/gbcurbrsr.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.hesvh.cn/Article/details/grerjwubf.sHtML

[R70] 时间戳与互转
来源：http://mobile.zdbjq.cn/Article/details/gybiymntd.sHtML

date +%s;  date -d @1700000000
来源：http://baike.hesvh.cn/Article/details/gcjdrnpcc.sHtML

[R71] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gmkxtutfv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/gkkvgygbf.sHtML

[R72] 等待端口就绪
来源：http://www.share.fehbvm.com/Article/details/gdqlzsfxp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gelkzqmfe.sHtML

[R73] 分割大日志
来源：http://blog.hesvh.cn/Article/details/grwvkputz.sHtML

split -l 1000 big.log part_
来源：http://m.share.hesvh.cn/Article/details/gujqmcnkb.sHtML

[R74] 批量重命名
来源：http://www.share.hesvh.cn/Article/details/gakubeyut.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/gtzepmilc.sHtML

[R75] 导出环境变量
来源：http://read.share.zdbjq.cn/Article/details/guxbovtko.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fehbvm.com/Article/details/gyozguyyz.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/ghagvejla.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gfzupcprx.sHtML

[R77] 读取用户输入
来源：http://blog.hesvh.cn/Article/details/gbtlipsqp.sHtML

read -rp "请输入: " ans
来源：http://m.share.fehbvm.com/Article/details/gzlmljmjh.sHtML

[R78] 交互式菜单
来源：http://baike.zdbjq.cn/Article/details/gcgmrzkfx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fehbvm.com/Article/details/gcpipvqyz.sHtML

[R79] 解析命令行选项
来源：http://www.blog.hesvh.cn/Article/details/gatnpocrw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fehbvm.com/Article/details/geqnolahs.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.hesvh.cn/Article/details/gimevwxff.sHtML

time ./run.sh
来源：http://www.m.share.zdbjq.cn/Article/details/gunybokxl.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxxheuumk.sHtML

S. C / C++ 专题
来源：http://www.blog.zdbjq.cn/Article/details/grvcedbph.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/godqtvhzh.sHtML

[S01] C：Hello World
来源：http://3g.hesvh.cn/Article/details/gxjjkfnjx.sHtML

#include <stdio.h>
来源：http://mobile.hesvh.cn/Article/details/gmpyomhep.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fehbvm.com/Article/details/gjtsqwgac.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.zdbjq.cn/Article/details/gwchgovbd.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fehbvm.com/Article/details/gxmavpgrj.sHtML

[S03] C：读入整数
来源：http://www.share.zdbjq.cn/Article/details/gwobyypqx.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fehbvm.com/Article/details/gxqvcnnkr.sHtML

[S04] C：字符串复制
来源：http://www.share.zdbjq.cn/Article/details/ghaoohbbp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fehbvm.com/Article/details/gzyykrfpn.sHtML

[S05] C：字符串长度
来源：http://wap.zdbjq.cn/Article/details/gaflzazpa.sHtML

strlen(s)
来源：http://3g.hesvh.cn/Article/details/gifecbcuf.sHtML

[S06] C：字符串比较
来源：http://mobile.fehbvm.com/Article/details/gwvepseum.sHtML

strcmp(a, b) == 0
来源：http://baike.hesvh.cn/Article/details/gelseovsg.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/gagymsosv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.hesvh.cn/Article/details/gumtucjcq.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/gnmpffnut.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fehbvm.com/Article/details/giirzqkug.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fehbvm.com/Article/details/gxqvzanbi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fehbvm.com/Article/details/gdvajfsat.sHtML

[S10] C：指针与解引用
来源：http://m.share.fehbvm.com/Article/details/gzdicnmxk.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/gipnqqkwv.sHtML

[S11] C：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gyagckgkg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fehbvm.com/Article/details/gewsivftj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gxvyaompf.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gwshfusrw.sHtML

[S12] C：写文件
来源：http://baike.fehbvm.com/Article/details/gmkwtaxbe.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gbbiqxbzy.sHtML

[S13] C：宏定义
来源：http://read.share.hesvh.cn/Article/details/gxvowopxg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fehbvm.com/Article/details/ggjkcbxuu.sHtML

[S14] C：枚举
来源：http://www.blog.fehbvm.com/Article/details/gmteybgrd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fehbvm.com/Article/details/glgtktpgi.sHtML

[S15] C：类型转换
来源：http://mobile.zdbjq.cn/Article/details/gnyeaekbs.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/ghokekhmt.sHtML

[S16] C：位操作置位
来源：http://www.share.hesvh.cn/Article/details/gcgaxofyl.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/ghkrjhubg.sHtML

[S17] C：安全拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gorfodzlr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fehbvm.com/Article/details/gipzylpii.sHtML

[S18] C：命令行参数
来源：http://mobile.hesvh.cn/Article/details/gshyffcby.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/gfxtmjves.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/gkdyoiqof.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/ghnjxknyc.sHtML

[S20] C：二分查找
来源：http://3g.fehbvm.com/Article/details/gbgevdpee.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/ggfwxylep.sHtML

[S21] C：字符类别判断
来源：http://mobile.fehbvm.com/Article/details/gaqrvbkwq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/gfvrgihrm.sHtML

[S22] C：字符串转数字
来源：http://3g.zdbjq.cn/Article/details/glmoxgzdm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/glogwpgyv.sHtML

[S23] C：随机数
来源：http://www.m.share.fehbvm.com/Article/details/ghpmqaxup.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.zdbjq.cn/Article/details/gretovdax.sHtML

[S24] C：获取本地时间
来源：http://www.blog.zdbjq.cn/Article/details/gbyjapmip.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.zdbjq.cn/Article/details/gxnseorrf.sHtML

[S25] C：内存拷贝
来源：http://read.share.hesvh.cn/Article/details/gxorxkywo.sHtML

memcpy(dst, src, n);
来源：http://mobile.fehbvm.com/Article/details/glfcejlqj.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/gxpakuncq.sHtML

memset(a, 0, sizeof a);
来源：http://wap.zdbjq.cn/Article/details/gpdksvnos.sHtML

[S27] C：定义常量
来源：http://wap.zdbjq.cn/Article/details/gqkkhgcfg.sHtML

const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gavfeofia.sHtML

[S28] C：静态变量
来源：http://blog.hesvh.cn/Article/details/gwotepzbu.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/ghzpfjqmi.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/gpnjerrwd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fehbvm.com/Article/details/gtlgnkwev.sHtML

[S30] C：头文件保护
来源：http://3g.zdbjq.cn/Article/details/ghwvfdrmp.sHtML

#ifndef X_H
来源：http://www.blog.fehbvm.com/Article/details/gwdqyylzs.sHtML

#define X_H
来源：http://www.share.zdbjq.cn/Article/details/gzreorwhb.sHtML

#endif
来源：http://www.blog.zdbjq.cn/Article/details/gysgnljps.sHtML

[S31] C++：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gjelkpzfr.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/gtwskvejm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.hesvh.cn/Article/details/gufslbvrv.sHtML

[S32] C++：字符串
来源：http://blog.zdbjq.cn/Article/details/gktyemima.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/gdqeusdxw.sHtML

[S33] C++：vector 增删
来源：http://www.share.fehbvm.com/Article/details/ghtkosdjw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.hesvh.cn/Article/details/gxufjjgcd.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/gruxzarzp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/gtoyynuke.sHtML

[S35] C++：map
来源：http://www.m.share.zdbjq.cn/Article/details/geawkamzl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gtkxyjfmh.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/gblhkgyff.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gzxjkrhsg.sHtML

[S37] C++：set
来源：http://www.share.zdbjq.cn/Article/details/gxyomfelb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/ggqapnpfk.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/gvfgtyewy.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.hesvh.cn/Article/details/gmwrnibyh.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fehbvm.com/Article/details/glxaayydx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.zdbjq.cn/Article/details/gnwrevkud.sHtML

[S40] C++：查找元素
来源：http://mobile.fehbvm.com/Article/details/grmrohwkt.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.zdbjq.cn/Article/details/gdffkgyes.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.hesvh.cn/Article/details/gikvrijit.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fehbvm.com/Article/details/gziwofgda.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/gjrepxnck.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.zdbjq.cn/Article/details/gsehqmijs.sHtML

[S43] C++：智能指针
来源：http://www.m.share.hesvh.cn/Article/details/gxsphsfur.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fehbvm.com/Article/details/gajyfeugu.sHtML

[S44] C++：引用传参
来源：http://baike.hesvh.cn/Article/details/gfxxudkud.sHtML

void inc(int &x) { ++x; }
来源：http://3g.hesvh.cn/Article/details/gwsvhjpri.sHtML

[S45] C++：lambda
来源：http://m.share.fehbvm.com/Article/details/ggenffyyx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.hesvh.cn/Article/details/gwudxjagq.sHtML

[S46] C++：函数模板
来源：http://wap.zdbjq.cn/Article/details/gkolsudkv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/ghrtkgodn.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/gjxjpkspe.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.zdbjq.cn/Article/details/gudqmygkv.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gsdynsxck.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.hesvh.cn/Article/details/grbvsbrsr.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fehbvm.com/Article/details/gphbhlucq.sHtML

[S49] C++：写文件
来源：http://mobile.hesvh.cn/Article/details/gtmsahuii.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fehbvm.com/Article/details/gwxkgatqp.sHtML

[S50] C++：格式化数字
来源：http://read.share.zdbjq.cn/Article/details/gnththajv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fehbvm.com/Article/details/ggampnrwq.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fehbvm.com/Article/details/gxzidxuhj.sHtML

static_cast<double>(a) / b
来源：http://blog.fehbvm.com/Article/details/gtssqmtvn.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fehbvm.com/Article/details/ggmuzukcz.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.zdbjq.cn/Article/details/gqdckqlmu.sHtML

[S53] C++：移动语义
来源：http://www.share.fehbvm.com/Article/details/gxtrsrbzq.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fehbvm.com/Article/details/gszvvgzlc.sHtML

[S54] C++：异常处理
来源：http://m.share.zdbjq.cn/Article/details/gbuzclcvo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.zdbjq.cn/Article/details/gerqppdss.sHtML

[S55] C++：结构化绑定
来源：http://read.share.hesvh.cn/Article/details/giqcrmlhk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.zdbjq.cn/Article/details/gezzreyaj.sHtML

[S56] C++：optional
来源：http://www.share.hesvh.cn/Article/details/gnjwyptfw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/grpurtrdr.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fehbvm.com/Article/details/gpsbehkhd.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/gigikyjup.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fehbvm.com/Article/details/goqjrrcgr.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fehbvm.com/Article/details/gmnouxouw.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/glhcbdhek.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fehbvm.com/Article/details/gwyubqnwt.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fehbvm.com/Article/details/grrkhzjii.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gxuzqdpax.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfrzymnbn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/gsvrkywfx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkwojpfdd.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fehbvm.com/Article/details/gayumjcef.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gbqwsryjs.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/gadfbwiyp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/gtftwdjqc.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/gqppvrzxb.sHtML

"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gewwmpced.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fehbvm.com/Article/details/gqefelkbx.sHtML

val n: String? = null;  n?.length
来源：http://www.share.hesvh.cn/Article/details/gnxmexsfr.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.zdbjq.cn/Article/details/gdssfbsbt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/gnkokdety.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fehbvm.com/Article/details/gxnljtmiq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.hesvh.cn/Article/details/gzpbzdlri.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.hesvh.cn/Article/details/gyxaenufh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gnneeayje.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/gbwichzcc.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fehbvm.com/Article/details/gmmhgkkhz.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.hesvh.cn/Article/details/giunfsssk.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.zdbjq.cn/Article/details/gbtsvffdc.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gvserhola.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/gegoavwpx.sHtML

[T11] Kotlin：协程
来源：http://www.blog.hesvh.cn/Article/details/gkjkeiecw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fehbvm.com/Article/details/gphrtdxbs.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fehbvm.com/Article/details/gflyftyyr.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gamvqmvvs.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.hesvh.cn/Article/details/gqrajvbkv.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fehbvm.com/Article/details/gtwgltoba.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fehbvm.com/Article/details/gmfaqwkdx.sHtML

for (i in 1..10) println(i)
来源：http://blog.fehbvm.com/Article/details/gpqqnhrqn.sHtML

[T15] Kotlin：接口
来源：http://baike.hesvh.cn/Article/details/gduhdrcip.sHtML

interface Shape { fun area(): Double }
来源：http://3g.hesvh.cn/Article/details/gkcbfukti.sHtML

[T16] Swift：Hello World
来源：http://3g.fehbvm.com/Article/details/gomicosfh.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/guorgaozf.sHtML

[T17] Swift：变量与常量
来源：http://3g.fehbvm.com/Article/details/gmyuchcnl.sHtML

var a = 1;  let b = 2
来源：http://blog.hesvh.cn/Article/details/gdboqnzfv.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gagbwzzyj.sHtML

"值: \(b)"
来源：http://mobile.zdbjq.cn/Article/details/gqhfbcqdu.sHtML

[T19] Swift：可选绑定
来源：http://baike.zdbjq.cn/Article/details/gjeblkuum.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/giofubpdh.sHtML

[T20] Swift：数组操作
来源：http://wap.fehbvm.com/Article/details/gtyysosma.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fehbvm.com/Article/details/giapvahlt.sHtML

[T21] Swift：遍历
来源：http://www.share.fehbvm.com/Article/details/galvnvwto.sHtML

for x in a { print(x) }
来源：http://3g.hesvh.cn/Article/details/gpeejpgqt.sHtML

[T22] Swift：字典
来源：http://m.share.fehbvm.com/Article/details/gknrgohwg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fehbvm.com/Article/details/gvzbofrdy.sHtML

[T23] Swift：函数
来源：http://wap.hesvh.cn/Article/details/gwwoojuqs.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fehbvm.com/Article/details/guskglcvn.sHtML

[T24] Swift：闭包
来源：http://mobile.hesvh.cn/Article/details/golykgfny.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fehbvm.com/Article/details/grnrxbcsg.sHtML

[T25] Swift：结构体
来源：http://blog.fehbvm.com/Article/details/gdptxvyiu.sHtML

struct P { var x: Int }
来源：http://www.m.share.fehbvm.com/Article/details/gyocztjqx.sHtML

[T26] Swift：类与重写
来源：http://read.share.hesvh.cn/Article/details/ggmaspryz.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.zdbjq.cn/Article/details/gxqpypeec.sHtML

[T27] Swift：错误处理
来源：http://mobile.fehbvm.com/Article/details/guzlatowd.sHtML

do { try f() } catch { print(error) }
来源：http://wap.hesvh.cn/Article/details/gmmyulxtz.sHtML

[T28] Swift：枚举
来源：http://wap.zdbjq.cn/Article/details/gbsrahyxf.sHtML

enum Color { case red, green }
来源：http://m.share.fehbvm.com/Article/details/gubcjmzmh.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.fehbvm.com/Article/details/gbmfxcahm.sHtML

guard let x = opt else { return }
来源：http://wap.hesvh.cn/Article/details/gqiijhrku.sHtML

[T30] Swift：协议
来源：http://www.blog.fehbvm.com/Article/details/ggiwhkcap.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.zdbjq.cn/Article/details/gvtbjgizz.sHtML

[T31] Lua：Hello World
来源：http://wap.hesvh.cn/Article/details/gnqgnribl.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gkwkpdffe.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gxnkrlajd.sHtML

local a = 1
来源：http://3g.zdbjq.cn/Article/details/gvgphulpu.sHtML


<!-- 参考信息 -->