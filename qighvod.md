代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://www.share.hesvh.cn/Article/details/gkoltgeuj.sHtML

[R32] 参数个数校验
来源：http://mobile.fehbvm.com/Article/details/gyuoedfek.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gxfwuacuf.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fehbvm.com/Article/details/gyfhfreky.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fehbvm.com/Article/details/guzjfixwe.sHtML

[R34] 退出时清理
来源：http://www.m.share.fehbvm.com/Article/details/glqqusnfb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/giggdijrq.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/gmnyemzfd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fehbvm.com/Article/details/ganowbelf.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fehbvm.com/Article/details/gdjjgmgts.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fehbvm.com/Article/details/gsavlabff.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fehbvm.com/Article/details/gpffbjzea.sHtML

files=$(ls -1)
来源：http://www.share.hesvh.cn/Article/details/gystfgddk.sHtML

[R38] 管道串联
来源：http://blog.hesvh.cn/Article/details/grnrpzked.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.hesvh.cn/Article/details/gpcuvdsrd.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/geemcocqm.sHtML

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/ghapfplng.sHtML

[R40] 追加写日志
来源：http://www.m.share.hesvh.cn/Article/details/gunxsznhb.sHtML

echo "log" >> out.log
来源：http://mobile.fehbvm.com/Article/details/ghuezsjks.sHtML

[R41] 丢弃输出
来源：http://wap.fehbvm.com/Article/details/gshljdhic.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/grjsdxxxj.sHtML

[R42] 输入重定向
来源：http://baike.zdbjq.cn/Article/details/gydtlctyn.sHtML

wc -l < a.txt
来源：http://3g.hesvh.cn/Article/details/ghcrqpgwz.sHtML

[R43] 按名字查找文件
来源：http://www.share.hesvh.cn/Article/details/gktagtalo.sHtML

find . -name "*.log" -type f
来源：http://3g.fehbvm.com/Article/details/gromsebux.sHtML

[R44] 按修改时间查找
来源：http://baike.zdbjq.cn/Article/details/grjqbozbv.sHtML

find . -mtime -7 -type f
来源：http://www.share.hesvh.cn/Article/details/ggvgmyxhg.sHtML

[R45] 批量删除
来源：http://m.share.hesvh.cn/Article/details/gtrheqfgg.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fehbvm.com/Article/details/gxhmleorm.sHtML

[R46] 递归替换文件内容
来源：http://wap.hesvh.cn/Article/details/gnnqvprtv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.zdbjq.cn/Article/details/giglznatb.sHtML

[R47] sed 单行替换
来源：http://mobile.fehbvm.com/Article/details/gzwgvypfr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.hesvh.cn/Article/details/gnnserpog.sHtML

[R48] awk 取指定列
来源：http://wap.fehbvm.com/Article/details/gvkoklxlh.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gohyfcwdc.sHtML

[R49] awk 带条件
来源：http://www.share.hesvh.cn/Article/details/glheaizhh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fehbvm.com/Article/details/gdfivpaqq.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/gamofipii.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fehbvm.com/Article/details/ggyilkdoh.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/grfinxolg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gauhwigtt.sHtML

[R52] 统计行数
来源：http://m.share.hesvh.cn/Article/details/gdbrffaer.sHtML

wc -l a.txt
来源：http://read.share.zdbjq.cn/Article/details/gxahadyww.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/gluicdvnc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/gazgvwsew.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/gdtdwcbde.sHtML

diff a.txt b.txt
来源：http://www.m.share.hesvh.cn/Article/details/gtihxebsp.sHtML

[R55] 压缩与解压
来源：http://mobile.fehbvm.com/Article/details/gvxhwvotk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/gzhmxqywt.sHtML

[R56] 远程拷贝
来源：http://baike.fehbvm.com/Article/details/gxilimicv.sHtML

scp file user@host:/path/
来源：http://read.share.zdbjq.cn/Article/details/gtybevtpz.sHtML

[R57] 远程执行命令
来源：http://m.share.fehbvm.com/Article/details/gociemaww.sHtML

ssh user@host 'uptime'
来源：http://3g.zdbjq.cn/Article/details/gzmpcgmkg.sHtML

[R58] 下载文件
来源：http://blog.hesvh.cn/Article/details/gvqnsbkaw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/grrpuxmnt.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gpatdutzp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fehbvm.com/Article/details/gloxztlkd.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/geyjnmbzu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/gzuoaobvj.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/gfsjjlidc.sHtML

df -h;  du -sh *
来源：http://www.m.share.zdbjq.cn/Article/details/gvvcchcjw.sHtML

[R62] 找最占空间的文件
来源：http://mobile.zdbjq.cn/Article/details/gknidpomy.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fehbvm.com/Article/details/giwxqbjhl.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/gcpsypycc.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.hesvh.cn/Article/details/gyujcxyut.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/gxdccrbvl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fehbvm.com/Article/details/gdlfilahv.sHtML

[R65] 查看端口占用
来源：http://wap.hesvh.cn/Article/details/gflbburpc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.zdbjq.cn/Article/details/gqilutnyv.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/ghndxqnkf.sHtML

crontab -e;  crontab -l
来源：http://read.share.hesvh.cn/Article/details/gvrykazey.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fehbvm.com/Article/details/gicbqyhxm.sHtML

openssl rand -hex 16
来源：http://read.share.zdbjq.cn/Article/details/gaegiimxi.sHtML

[R68] 计算文件校验值
来源：http://wap.zdbjq.cn/Article/details/gaqhkwwxr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.hesvh.cn/Article/details/gmgpyzpuq.sHtML

[R69] 生成随机密码
来源：http://blog.hesvh.cn/Article/details/grosrqppg.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/goukpxevy.sHtML

[R70] 时间戳与互转
来源：http://3g.zdbjq.cn/Article/details/glauygepl.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fehbvm.com/Article/details/gjwybyhig.sHtML

[R71] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gwejjrdfv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.zdbjq.cn/Article/details/gfzxbxcke.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/giscqmxyl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gnvsszoqw.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/gokdlmlly.sHtML

split -l 1000 big.log part_
来源：http://wap.zdbjq.cn/Article/details/gttzjtifg.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/gcjpecmmq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.zdbjq.cn/Article/details/ggmhlzlss.sHtML

[R75] 导出环境变量
来源：http://3g.hesvh.cn/Article/details/gbwaynrjm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.zdbjq.cn/Article/details/gvfkoqtsm.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/gfyrluuzx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gehfmvuaq.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/gsjvhvxuy.sHtML

read -rp "请输入: " ans
来源：http://mobile.hesvh.cn/Article/details/gpbflfwrd.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/gyopueaho.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.hesvh.cn/Article/details/grbmuotgs.sHtML

[R79] 解析命令行选项
来源：http://mobile.hesvh.cn/Article/details/gnatpwgyg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fehbvm.com/Article/details/gztwofvgf.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fehbvm.com/Article/details/gmnrhwkbc.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/gkmxkvvkv.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxasqrbwh.sHtML

S. C / C++ 专题
来源：http://blog.hesvh.cn/Article/details/gyaqtedqv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwnsabwvz.sHtML

[S01] C：Hello World
来源：http://wap.zdbjq.cn/Article/details/gglhgvnea.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/girisodce.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gahxnzeoi.sHtML

[S02] C：变量与格式化输出
来源：http://baike.hesvh.cn/Article/details/gygdgrfne.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/gcsqjfptr.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/gsopwslse.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/gtaeeuspb.sHtML

[S04] C：字符串复制
来源：http://www.share.zdbjq.cn/Article/details/gmzdqntgi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fehbvm.com/Article/details/gxzzyrard.sHtML

[S05] C：字符串长度
来源：http://3g.hesvh.cn/Article/details/gthggjdhj.sHtML

strlen(s)
来源：http://m.share.zdbjq.cn/Article/details/gxyvyylvq.sHtML

[S06] C：字符串比较
来源：http://baike.hesvh.cn/Article/details/gmtufgrzr.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/gpldoopta.sHtML

[S07] C：数组遍历求和
来源：http://baike.hesvh.cn/Article/details/gqfrbrgkc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fehbvm.com/Article/details/gswhzipkz.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.hesvh.cn/Article/details/ginkgqhuo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.hesvh.cn/Article/details/grmsncrgw.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/gpqaweiqe.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fehbvm.com/Article/details/gpeevznnk.sHtML

[S10] C：指针与解引用
来源：http://mobile.fehbvm.com/Article/details/gybsmdudk.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gadnkmdye.sHtML

[S11] C：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gwonyomdv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.zdbjq.cn/Article/details/gbsbobbda.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/gkwvivbby.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/gewlutzhu.sHtML

[S12] C：写文件
来源：http://3g.fehbvm.com/Article/details/glzbgsgts.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gnatxayal.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/gdpbguiuo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/gjadyyefl.sHtML

[S14] C：枚举
来源：http://read.share.hesvh.cn/Article/details/grfzjogtt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.hesvh.cn/Article/details/gtcanvzta.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/gxklpkjov.sHtML

(double) a / b
来源：http://wap.zdbjq.cn/Article/details/gpqnnzjso.sHtML

[S16] C：位操作置位
来源：http://mobile.hesvh.cn/Article/details/gbotexiui.sHtML

x |= (1 << 3);
来源：http://baike.fehbvm.com/Article/details/gcqalnpxm.sHtML

[S17] C：安全拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gfycobjff.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/gmzroissj.sHtML

[S18] C：命令行参数
来源：http://mobile.hesvh.cn/Article/details/gelcspylf.sHtML

int main(int argc, char **argv)
来源：http://3g.zdbjq.cn/Article/details/gqemwcrxn.sHtML

[S19] C：快速排序
来源：http://3g.hesvh.cn/Article/details/gnqqtxeco.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/ghftsnual.sHtML

[S20] C：二分查找
来源：http://baike.fehbvm.com/Article/details/gyysyweql.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/ggyvwixlv.sHtML

[S21] C：字符类别判断
来源：http://mobile.fehbvm.com/Article/details/ggqhzvmpc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/gnyrcvygo.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/gejdtnsgy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fehbvm.com/Article/details/grmppmyvx.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/gmxehpijk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fehbvm.com/Article/details/gkjtnduny.sHtML

[S24] C：获取本地时间
来源：http://read.share.fehbvm.com/Article/details/gsirvncyy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/gmxkxcsfw.sHtML

[S25] C：内存拷贝
来源：http://mobile.fehbvm.com/Article/details/gxvkpjrer.sHtML

memcpy(dst, src, n);
来源：http://3g.fehbvm.com/Article/details/gztfbzyaz.sHtML

[S26] C：内存清零
来源：http://www.m.share.zdbjq.cn/Article/details/gntwkoltq.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.zdbjq.cn/Article/details/gcjjfnodc.sHtML

[S27] C：定义常量
来源：http://blog.fehbvm.com/Article/details/guzlehick.sHtML

const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gakmvvnzm.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/gjsfjltso.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/gvcyhluoq.sHtML

[S29] C：变参函数
来源：http://wap.hesvh.cn/Article/details/giktopper.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.zdbjq.cn/Article/details/gfovnnpnq.sHtML

[S30] C：头文件保护
来源：http://m.share.zdbjq.cn/Article/details/gksgdmxjy.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/gxnhvgirk.sHtML

#define X_H
来源：http://www.m.share.fehbvm.com/Article/details/gqismvzjy.sHtML

#endif
来源：http://m.share.hesvh.cn/Article/details/gdpxuupsf.sHtML

[S31] C++：Hello World
来源：http://wap.fehbvm.com/Article/details/gyiagzety.sHtML

#include <iostream>
来源：http://m.share.fehbvm.com/Article/details/gptcvdlyn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/glddpcgat.sHtML

[S32] C++：字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gavszykpj.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fehbvm.com/Article/details/gulnniqfm.sHtML

[S33] C++：vector 增删
来源：http://read.share.zdbjq.cn/Article/details/gccvltwyo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/gxoqtefwy.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/gbofgsucw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/gdcotnbqn.sHtML

[S35] C++：map
来源：http://3g.fehbvm.com/Article/details/ghuivtwdh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gomvvxolr.sHtML

[S36] C++：unordered_map
来源：http://www.blog.hesvh.cn/Article/details/gueurlcot.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gtmsodddo.sHtML

[S37] C++：set
来源：http://mobile.hesvh.cn/Article/details/gxobkiklw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/glnlyskwf.sHtML

[S38] C++：排序
来源：http://www.m.share.zdbjq.cn/Article/details/gwmpbeyha.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fehbvm.com/Article/details/gdlojghnz.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.hesvh.cn/Article/details/ggwnkwlcc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fehbvm.com/Article/details/gkbxximyt.sHtML

[S40] C++：查找元素
来源：http://mobile.fehbvm.com/Article/details/ggaxhawid.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.zdbjq.cn/Article/details/gfcqamdbu.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fehbvm.com/Article/details/gdibirxvc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.zdbjq.cn/Article/details/grqkpjebi.sHtML

[S42] C++：继承与虚函数
来源：http://wap.zdbjq.cn/Article/details/gsgpcanxw.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.zdbjq.cn/Article/details/gofxzqdzr.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/gbvnncofb.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.hesvh.cn/Article/details/gwqdnjqcx.sHtML

[S44] C++：引用传参
来源：http://baike.fehbvm.com/Article/details/gdmojldla.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.hesvh.cn/Article/details/gtcatldbc.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/gipbgwlgi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/geftuapdh.sHtML

[S46] C++：函数模板
来源：http://www.m.share.zdbjq.cn/Article/details/gudfbhjml.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.zdbjq.cn/Article/details/gafazswhj.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fehbvm.com/Article/details/gdwzdgyja.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fehbvm.com/Article/details/gjpbaplfg.sHtML

[S48] C++：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gfgicdyku.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.hesvh.cn/Article/details/gpidosklb.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/gfbsdkdub.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/gjbguzwmt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.hesvh.cn/Article/details/gtpqqulsv.sHtML

[S50] C++：格式化数字
来源：http://3g.fehbvm.com/Article/details/gqmsiltma.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gjlqjtppn.sHtML

[S51] C++：显式类型转换
来源：http://baike.fehbvm.com/Article/details/gehlewrym.sHtML

static_cast<double>(a) / b
来源：http://3g.fehbvm.com/Article/details/gbgvpedjt.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.hesvh.cn/Article/details/gaerjxtmg.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/ghhzhpsfi.sHtML

[S53] C++：移动语义
来源：http://3g.zdbjq.cn/Article/details/gegziqihl.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.hesvh.cn/Article/details/gxxxoeecp.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/gxdawpiwf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.hesvh.cn/Article/details/gzssguejq.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fehbvm.com/Article/details/gturpbivn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.zdbjq.cn/Article/details/ggaqrsogm.sHtML

[S56] C++：optional
来源：http://mobile.zdbjq.cn/Article/details/gdsvoncxy.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/gvtcwhiyn.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fehbvm.com/Article/details/gxwinairz.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/gvpjpxcuh.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fehbvm.com/Article/details/ggffpoeef.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.hesvh.cn/Article/details/gjafvhbpw.sHtML

[S59] C++：静态断言
来源：http://blog.fehbvm.com/Article/details/gxbxezmfb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fehbvm.com/Article/details/guijufkal.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gwjptgzrf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fehbvm.com/Article/details/gzdmcuihj.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gourzlknl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/geqahvyze.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gpzjjnmnb.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.hesvh.cn/Article/details/gfxambwtn.sHtML

println("Hello")
来源：http://www.blog.fehbvm.com/Article/details/grdwqagfh.sHtML

[T02] Kotlin：变量
来源：http://read.share.fehbvm.com/Article/details/gspvaiebe.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.hesvh.cn/Article/details/gqopfrmtq.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.hesvh.cn/Article/details/giazvfryg.sHtML

"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gudjunapn.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.hesvh.cn/Article/details/gonftytkt.sHtML

val n: String? = null;  n?.length
来源：http://blog.zdbjq.cn/Article/details/goswwardi.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.hesvh.cn/Article/details/gwaghebty.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.fehbvm.com/Article/details/gcbotwrux.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fehbvm.com/Article/details/giiasklrq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.hesvh.cn/Article/details/gexiejpto.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gdkegnnea.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.zdbjq.cn/Article/details/gzimgqnxq.sHtML

[T08] Kotlin：数据类
来源：http://blog.zdbjq.cn/Article/details/giamrzisc.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.hesvh.cn/Article/details/gmqyhypmv.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.zdbjq.cn/Article/details/gezdngscv.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.zdbjq.cn/Article/details/giyyizele.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gteyaufqt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.hesvh.cn/Article/details/gkwjwisjx.sHtML

[T11] Kotlin：协程
来源：http://m.share.fehbvm.com/Article/details/gjpupugng.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://mobile.fehbvm.com/Article/details/gxmrnnhnz.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.zdbjq.cn/Article/details/gdcydwqir.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.hesvh.cn/Article/details/ghciggumh.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fehbvm.com/Article/details/gboeobcww.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fehbvm.com/Article/details/gyjpwlpvj.sHtML

[T14] Kotlin：循环
来源：http://baike.zdbjq.cn/Article/details/gxhbptult.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.hesvh.cn/Article/details/ghkyhgrku.sHtML

[T15] Kotlin：接口
来源：http://m.share.fehbvm.com/Article/details/gwyljyild.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fehbvm.com/Article/details/gvrxhtdrm.sHtML

[T16] Swift：Hello World
来源：http://wap.zdbjq.cn/Article/details/gukuwnmda.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/guiryygfm.sHtML

[T17] Swift：变量与常量
来源：http://3g.fehbvm.com/Article/details/ggjdeubmk.sHtML

var a = 1;  let b = 2
来源：http://baike.hesvh.cn/Article/details/gdcbmnpdb.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gjxyzckef.sHtML

"值: \(b)"
来源：http://read.share.fehbvm.com/Article/details/gidgjxjow.sHtML

[T19] Swift：可选绑定
来源：http://www.share.zdbjq.cn/Article/details/gzrhlqxqp.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fehbvm.com/Article/details/gldvxenrm.sHtML

[T20] Swift：数组操作
来源：http://blog.fehbvm.com/Article/details/gztlfarub.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.zdbjq.cn/Article/details/gxqxhjqfd.sHtML

[T21] Swift：遍历
来源：http://3g.zdbjq.cn/Article/details/gcnlpccsy.sHtML

for x in a { print(x) }
来源：http://3g.fehbvm.com/Article/details/gnmiexori.sHtML

[T22] Swift：字典
来源：http://mobile.fehbvm.com/Article/details/gfkiijgpv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.hesvh.cn/Article/details/gxzbdmesp.sHtML

[T23] Swift：函数
来源：http://baike.fehbvm.com/Article/details/gwotyvlzs.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.hesvh.cn/Article/details/gpunejxwt.sHtML

[T24] Swift：闭包
来源：http://www.blog.fehbvm.com/Article/details/ginotrgyj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fehbvm.com/Article/details/gjdmonlat.sHtML

[T25] Swift：结构体
来源：http://www.share.zdbjq.cn/Article/details/ghzdcqxhe.sHtML

struct P { var x: Int }
来源：http://blog.fehbvm.com/Article/details/gojktqvmf.sHtML

[T26] Swift：类与重写
来源：http://3g.fehbvm.com/Article/details/gjgzpxelg.sHtML

class A: Base { override func f() {} }
来源：http://baike.zdbjq.cn/Article/details/gilocafhr.sHtML

[T27] Swift：错误处理
来源：http://mobile.fehbvm.com/Article/details/gefwsvdrf.sHtML

do { try f() } catch { print(error) }
来源：http://wap.hesvh.cn/Article/details/gnpeaaiiv.sHtML

[T28] Swift：枚举
来源：http://www.share.zdbjq.cn/Article/details/gggdqfhcd.sHtML

enum Color { case red, green }
来源：http://3g.fehbvm.com/Article/details/gvzgtzfaa.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/ghsdlpyly.sHtML

guard let x = opt else { return }
来源：http://wap.zdbjq.cn/Article/details/gmqdtkjut.sHtML

[T30] Swift：协议
来源：http://wap.zdbjq.cn/Article/details/gauezbkuh.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.zdbjq.cn/Article/details/gjstqurzr.sHtML

[T31] Lua：Hello World
来源：http://wap.hesvh.cn/Article/details/gywcllsvr.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gkkibbynb.sHtML

[T32] Lua：局部变量
来源：http://3g.hesvh.cn/Article/details/gnhrlvhyq.sHtML

local a = 1
来源：http://wap.hesvh.cn/Article/details/geogqqzbq.sHtML

[T33] Lua：表（数组）
来源：http://3g.fehbvm.com/Article/details/gtsdxnuhn.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.fehbvm.com/Article/details/ggyqbrpzl.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.hesvh.cn/Article/details/gygmwtqfl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fehbvm.com/Article/details/gsmdpqfla.sHtML


<!-- 参考信息 -->