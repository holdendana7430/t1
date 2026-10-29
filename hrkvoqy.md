代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://3g.fehbvm.com/Article/details/gizjtkees.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/gkjjquftu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gitfomiop.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.hesvh.cn/Article/details/gwgryndkd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.hesvh.cn/Article/details/giwdjjswd.sHtML

[R34] 退出时清理
来源：http://baike.zdbjq.cn/Article/details/gnhbkrybr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gjebedjqy.sHtML

[R35] 后台执行并等待
来源：http://wap.hesvh.cn/Article/details/gooenhbmb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.hesvh.cn/Article/details/gstkrhhhe.sHtML

[R36] 并发执行多个任务
来源：http://3g.hesvh.cn/Article/details/gbvbtpijr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fehbvm.com/Article/details/ghdolobhk.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.hesvh.cn/Article/details/gfjmslmuj.sHtML

files=$(ls -1)
来源：http://blog.zdbjq.cn/Article/details/ghxokjnzs.sHtML

[R38] 管道串联
来源：http://blog.hesvh.cn/Article/details/gsymjurvg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.zdbjq.cn/Article/details/gzdafqyyw.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/gasaricux.sHtML

cmd > out.log 2>&1
来源：http://read.share.fehbvm.com/Article/details/gbnvmmqcc.sHtML

[R40] 追加写日志
来源：http://wap.hesvh.cn/Article/details/gzkkogoad.sHtML

echo "log" >> out.log
来源：http://read.share.hesvh.cn/Article/details/gslmivgyo.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/gsksbywgi.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gbzzjjssh.sHtML

[R42] 输入重定向
来源：http://www.blog.fehbvm.com/Article/details/gyjcewggd.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/gqjgtnxvy.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/gjjrxoezk.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gbsmqrifo.sHtML

[R44] 按修改时间查找
来源：http://3g.zdbjq.cn/Article/details/gmmpgkxto.sHtML

find . -mtime -7 -type f
来源：http://wap.zdbjq.cn/Article/details/gjnwczkqq.sHtML

[R45] 批量删除
来源：http://www.blog.fehbvm.com/Article/details/gtdspbpnr.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.zdbjq.cn/Article/details/gwibhfhmg.sHtML

[R46] 递归替换文件内容
来源：http://3g.hesvh.cn/Article/details/gcdmawruw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fehbvm.com/Article/details/gomhzpwql.sHtML

[R47] sed 单行替换
来源：http://www.m.share.zdbjq.cn/Article/details/gxzphuqug.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/guiybnrhx.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gfqniuibr.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.hesvh.cn/Article/details/gytzdpoag.sHtML

[R49] awk 带条件
来源：http://m.share.hesvh.cn/Article/details/gxewuookc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fehbvm.com/Article/details/gwstlecsk.sHtML

[R50] awk 求和
来源：http://read.share.fehbvm.com/Article/details/guibdlgwe.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.hesvh.cn/Article/details/gntoybidr.sHtML

[R51] 排序去重取前几
来源：http://m.share.fehbvm.com/Article/details/gybuvpiki.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fehbvm.com/Article/details/gasjrwmer.sHtML

[R52] 统计行数
来源：http://3g.zdbjq.cn/Article/details/gtrcmflta.sHtML

wc -l a.txt
来源：http://wap.fehbvm.com/Article/details/gkrtekwbq.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.zdbjq.cn/Article/details/gbhfjnxlb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fehbvm.com/Article/details/gqcnlzteq.sHtML

[R54] 比较两个文件
来源：http://baike.hesvh.cn/Article/details/gbdxrhcya.sHtML

diff a.txt b.txt
来源：http://www.share.hesvh.cn/Article/details/gdmgocqfl.sHtML

[R55] 压缩与解压
来源：http://m.share.fehbvm.com/Article/details/gdzkidvlk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.hesvh.cn/Article/details/gbjsddrgb.sHtML

[R56] 远程拷贝
来源：http://m.share.fehbvm.com/Article/details/gfnxaymas.sHtML

scp file user@host:/path/
来源：http://wap.zdbjq.cn/Article/details/gjdbabvgm.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/gyogjdkar.sHtML

ssh user@host 'uptime'
来源：http://www.blog.zdbjq.cn/Article/details/gscbdwnkl.sHtML

[R58] 下载文件
来源：http://mobile.fehbvm.com/Article/details/gjebtxohy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fehbvm.com/Article/details/gfxozmznk.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/giavogaen.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/gsqzmgjti.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/ghidkerwe.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/gydauheqn.sHtML

[R61] 磁盘占用
来源：http://3g.fehbvm.com/Article/details/gnbpqeqwf.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/goagubqke.sHtML

[R62] 找最占空间的文件
来源：http://blog.fehbvm.com/Article/details/gweniaokc.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.zdbjq.cn/Article/details/grgxksbyi.sHtML

[R63] 内存与进程
来源：http://blog.hesvh.cn/Article/details/gkyxvhvrk.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fehbvm.com/Article/details/gynsjyhym.sHtML

[R64] 结束进程
来源：http://read.share.hesvh.cn/Article/details/gqqjgfjxl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.zdbjq.cn/Article/details/gipzghhdb.sHtML

[R65] 查看端口占用
来源：http://www.blog.fehbvm.com/Article/details/gkzpmpwlz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.hesvh.cn/Article/details/gzvvqgtoj.sHtML

[R66] 定时任务
来源：http://3g.hesvh.cn/Article/details/ghajksmnu.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/ggtstmoqp.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fehbvm.com/Article/details/gtxvoemnl.sHtML

openssl rand -hex 16
来源：http://baike.hesvh.cn/Article/details/gtpwxbztj.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/gflrxkeou.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.zdbjq.cn/Article/details/grxqcekdb.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/gfwbnbdax.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.zdbjq.cn/Article/details/gfhauxvjs.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/gdrxsdomw.sHtML

date +%s;  date -d @1700000000
来源：http://wap.zdbjq.cn/Article/details/ggicrbhmb.sHtML

[R71] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gosclecei.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gpdmzyiax.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.zdbjq.cn/Article/details/gzitkyaha.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gqkcxktyu.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/ggqvgszgm.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/gotasgcik.sHtML

[R74] 批量重命名
来源：http://m.share.fehbvm.com/Article/details/gmrnzzaui.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/gprilmcck.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gytzkbkfw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.hesvh.cn/Article/details/gfphpelsa.sHtML

[R76] 使用临时文件
来源：http://baike.hesvh.cn/Article/details/ghzqqbqlb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gfufhuact.sHtML

[R77] 读取用户输入
来源：http://wap.hesvh.cn/Article/details/gnjvygafu.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/gxvdsuvvq.sHtML

[R78] 交互式菜单
来源：http://www.m.share.hesvh.cn/Article/details/guyspfkyp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.zdbjq.cn/Article/details/gqnmddfvt.sHtML

[R79] 解析命令行选项
来源：http://wap.zdbjq.cn/Article/details/gajmesocs.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.zdbjq.cn/Article/details/giywoflda.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.zdbjq.cn/Article/details/gjpnhfrcj.sHtML

time ./run.sh
来源：http://www.m.share.zdbjq.cn/Article/details/geceznsle.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcrudpkjx.sHtML

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/gyzkgtfcu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbalmjkxm.sHtML

[S01] C：Hello World
来源：http://blog.zdbjq.cn/Article/details/gmxpikcld.sHtML

#include <stdio.h>
来源：http://blog.hesvh.cn/Article/details/gestdkfkc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fehbvm.com/Article/details/gnbjfikmg.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.hesvh.cn/Article/details/gptdzrjnq.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/gdzpqapae.sHtML

[S03] C：读入整数
来源：http://read.share.hesvh.cn/Article/details/gfkyumfer.sHtML

int x; scanf("%d", &x);
来源：http://mobile.zdbjq.cn/Article/details/gdqhtakcd.sHtML

[S04] C：字符串复制
来源：http://mobile.zdbjq.cn/Article/details/gpfuqlkyr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/gmnfdtfdd.sHtML

[S05] C：字符串长度
来源：http://baike.zdbjq.cn/Article/details/gwsfousxc.sHtML

strlen(s)
来源：http://m.share.hesvh.cn/Article/details/ghhtmqybj.sHtML

[S06] C：字符串比较
来源：http://m.share.hesvh.cn/Article/details/gcxvptedr.sHtML

strcmp(a, b) == 0
来源：http://mobile.zdbjq.cn/Article/details/ggsoydina.sHtML

[S07] C：数组遍历求和
来源：http://wap.fehbvm.com/Article/details/gtlrtnshu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.zdbjq.cn/Article/details/gbndzutty.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.zdbjq.cn/Article/details/gabdxephz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.hesvh.cn/Article/details/gelikhnrl.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/gcxxjypoy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fehbvm.com/Article/details/gzregidtu.sHtML

[S10] C：指针与解引用
来源：http://3g.fehbvm.com/Article/details/gwyfsxlxk.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fehbvm.com/Article/details/gbegiugii.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gacicdkss.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fehbvm.com/Article/details/gkhcigrzv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.hesvh.cn/Article/details/glzwaahsr.sHtML

fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/guymbppna.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/gqmeyohko.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gvjvqiiil.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/gwocffiuf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fehbvm.com/Article/details/gjnmhqtlc.sHtML

[S14] C：枚举
来源：http://blog.hesvh.cn/Article/details/gdgzwtpec.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.hesvh.cn/Article/details/goskfktbc.sHtML

[S15] C：类型转换
来源：http://baike.hesvh.cn/Article/details/garsrtoef.sHtML

(double) a / b
来源：http://wap.zdbjq.cn/Article/details/gasnqcena.sHtML

[S16] C：位操作置位
来源：http://wap.hesvh.cn/Article/details/gbgyqmkgr.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/gqtyjpeoq.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gjfxqaevm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/gtymysspm.sHtML

[S18] C：命令行参数
来源：http://wap.zdbjq.cn/Article/details/gtftkoivi.sHtML

int main(int argc, char **argv)
来源：http://read.share.hesvh.cn/Article/details/gmwefzqly.sHtML

[S19] C：快速排序
来源：http://www.m.share.hesvh.cn/Article/details/gdzqyjaww.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gxpvtvocr.sHtML

[S20] C：二分查找
来源：http://baike.fehbvm.com/Article/details/gqomfbdnn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gukoftkac.sHtML

[S21] C：字符类别判断
来源：http://wap.fehbvm.com/Article/details/gxqorvrmz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fehbvm.com/Article/details/gusioayjy.sHtML

[S22] C：字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/gwvhkxujx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fehbvm.com/Article/details/gcilehmqn.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/gczwgisbd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/gqqnooiqo.sHtML

[S24] C：获取本地时间
来源：http://m.share.fehbvm.com/Article/details/gvnyavuwv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.hesvh.cn/Article/details/ghlbfpqos.sHtML

[S25] C：内存拷贝
来源：http://wap.fehbvm.com/Article/details/gmkkzhram.sHtML

memcpy(dst, src, n);
来源：http://www.blog.zdbjq.cn/Article/details/gqirqowlu.sHtML

[S26] C：内存清零
来源：http://blog.fehbvm.com/Article/details/gtcjorwtx.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/gqkozrcja.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/gnyaoprrq.sHtML

const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gbwiazfnw.sHtML

[S28] C：静态变量
来源：http://m.share.zdbjq.cn/Article/details/gkswjyweb.sHtML

static int counter = 0;
来源：http://3g.fehbvm.com/Article/details/gqyyhamoh.sHtML

[S29] C：变参函数
来源：http://blog.hesvh.cn/Article/details/gtflzygfk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.hesvh.cn/Article/details/gkfgwljlh.sHtML

[S30] C：头文件保护
来源：http://www.blog.zdbjq.cn/Article/details/gwjdkaswv.sHtML

#ifndef X_H
来源：http://blog.zdbjq.cn/Article/details/gyszlenot.sHtML

#define X_H
来源：http://blog.hesvh.cn/Article/details/gncvwdgth.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/gfttoeype.sHtML

[S31] C++：Hello World
来源：http://mobile.fehbvm.com/Article/details/grivqtgxk.sHtML

#include <iostream>
来源：http://www.blog.zdbjq.cn/Article/details/ggphhbgqt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.zdbjq.cn/Article/details/goivpabmr.sHtML

[S32] C++：字符串
来源：http://www.share.hesvh.cn/Article/details/ggqngxnur.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.hesvh.cn/Article/details/gygosjlfi.sHtML

[S33] C++：vector 增删
来源：http://baike.fehbvm.com/Article/details/gimmzibva.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fehbvm.com/Article/details/gnpgkfpei.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/gsdwkioms.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fehbvm.com/Article/details/gflymmsjc.sHtML

[S35] C++：map
来源：http://blog.hesvh.cn/Article/details/grghpnouq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/golfmkxsa.sHtML

[S36] C++：unordered_map
来源：http://mobile.zdbjq.cn/Article/details/gnkifgjey.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gmbpofdoy.sHtML

[S37] C++：set
来源：http://baike.zdbjq.cn/Article/details/gevzkmfzh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fehbvm.com/Article/details/guwyurmcn.sHtML

[S38] C++：排序
来源：http://read.share.hesvh.cn/Article/details/gyimogntg.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gekauefov.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/ganislryn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.zdbjq.cn/Article/details/gcuolmhdi.sHtML

[S40] C++：查找元素
来源：http://www.m.share.zdbjq.cn/Article/details/gpmesxjww.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.zdbjq.cn/Article/details/grbzpkfom.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fehbvm.com/Article/details/gprhykjyd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.hesvh.cn/Article/details/ghvpvrinh.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/gjzjrxuux.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/gasuldxas.sHtML

[S43] C++：智能指针
来源：http://mobile.hesvh.cn/Article/details/gjejedssx.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.zdbjq.cn/Article/details/gbjwhbjmm.sHtML

[S44] C++：引用传参
来源：http://m.share.zdbjq.cn/Article/details/glmapgmim.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.zdbjq.cn/Article/details/gyeftcisf.sHtML

[S45] C++：lambda
来源：http://mobile.hesvh.cn/Article/details/gzohyekza.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/gabjhjkgc.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fehbvm.com/Article/details/gzbtiikmh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/gnlvixfug.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fehbvm.com/Article/details/gvudxkcbn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.zdbjq.cn/Article/details/gynwenfnc.sHtML

[S48] C++：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gvtfnqeoq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.hesvh.cn/Article/details/gdaqbqpuc.sHtML

while (std::getline(in, line)) { }
来源：http://baike.hesvh.cn/Article/details/gmjacenoo.sHtML

[S49] C++：写文件
来源：http://wap.hesvh.cn/Article/details/gbjbragvh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/gvpvuwdwd.sHtML

[S50] C++：格式化数字
来源：http://m.share.zdbjq.cn/Article/details/grrmueiwi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/ggdhnxwcz.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/glqujvizx.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fehbvm.com/Article/details/gxxwmwgwj.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.hesvh.cn/Article/details/gullfpuzv.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.hesvh.cn/Article/details/gqyuscqhz.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/ghypisnxm.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fehbvm.com/Article/details/gsttogxoo.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/gveozmabt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fehbvm.com/Article/details/grhmqybbu.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/gefipequx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fehbvm.com/Article/details/ggkdzzyhl.sHtML

[S56] C++：optional
来源：http://3g.fehbvm.com/Article/details/gcsklzoae.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/gboidytgj.sHtML

[S57] C++：编译期常量
来源：http://3g.zdbjq.cn/Article/details/gziecfqeb.sHtML

constexpr int N = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gsezukmkp.sHtML

[S58] C++：命名空间
来源：http://blog.fehbvm.com/Article/details/gpuzzgepm.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fehbvm.com/Article/details/ggcqrcgdx.sHtML

[S59] C++：静态断言
来源：http://m.share.hesvh.cn/Article/details/gnhdubfrc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.hesvh.cn/Article/details/gqjeebwxm.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fehbvm.com/Article/details/ghgemxivf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gbfkrkkxz.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkegsdebc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/ghmrlhcwg.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqnktpmtw.sHtML

[T01] Kotlin：Hello World
来源：http://blog.hesvh.cn/Article/details/gbkgzvzhh.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/gmhhgales.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/gndqwkzbe.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.zdbjq.cn/Article/details/glgfbxxjs.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fehbvm.com/Article/details/gnhwzutcy.sHtML

"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gegqozbcj.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/gfltjmrii.sHtML

val n: String? = null;  n?.length
来源：http://baike.fehbvm.com/Article/details/ggrmwukab.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.hesvh.cn/Article/details/gzaahvjqb.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.hesvh.cn/Article/details/giiqfutfy.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gchfnulwc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.zdbjq.cn/Article/details/gnxghrxyg.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.hesvh.cn/Article/details/giejekbiv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.zdbjq.cn/Article/details/gcgnrkzxo.sHtML

[T08] Kotlin：数据类
来源：http://read.share.hesvh.cn/Article/details/gsaydqckg.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fehbvm.com/Article/details/gjznjeqch.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/gmqafnpao.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.hesvh.cn/Article/details/guxyzvxfw.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gkxboubkr.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.zdbjq.cn/Article/details/gbcosbcwz.sHtML

[T11] Kotlin：协程
来源：http://m.share.zdbjq.cn/Article/details/gxsxtkmtp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/govrzgnha.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fehbvm.com/Article/details/gjuxmtnjc.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.hesvh.cn/Article/details/gpeqjncsy.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.zdbjq.cn/Article/details/gvqznbygy.sHtML

val m = mapOf("a" to 1)
来源：http://blog.zdbjq.cn/Article/details/gccecyebv.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/ggabkorgz.sHtML

for (i in 1..10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gbmlpiyrp.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.hesvh.cn/Article/details/ghibdjpux.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fehbvm.com/Article/details/gdkssmwww.sHtML

[T16] Swift：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gcttqoptd.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gxwqceiwa.sHtML

[T17] Swift：变量与常量
来源：http://mobile.hesvh.cn/Article/details/gsilnzhda.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gxpteinzl.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gwynvbedr.sHtML

"值: \(b)"
来源：http://3g.fehbvm.com/Article/details/gzziijdjy.sHtML

[T19] Swift：可选绑定
来源：http://wap.fehbvm.com/Article/details/gbrusuokh.sHtML

if let n = opt { print(n) }
来源：http://3g.hesvh.cn/Article/details/gqkqffckd.sHtML

[T20] Swift：数组操作
来源：http://3g.fehbvm.com/Article/details/gkbhvlagx.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/ghphgfjvz.sHtML

[T21] Swift：遍历
来源：http://www.share.fehbvm.com/Article/details/gzsptpvrt.sHtML

for x in a { print(x) }
来源：http://m.share.fehbvm.com/Article/details/gmkuoryfo.sHtML

[T22] Swift：字典
来源：http://mobile.hesvh.cn/Article/details/ggepjuyns.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.zdbjq.cn/Article/details/gutslazzw.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/gttietaxf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fehbvm.com/Article/details/ggnjpbede.sHtML

[T24] Swift：闭包
来源：http://wap.fehbvm.com/Article/details/gfjkrrrqs.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gsnfbrhty.sHtML

[T25] Swift：结构体
来源：http://wap.hesvh.cn/Article/details/gabgahzaq.sHtML

struct P { var x: Int }
来源：http://read.share.fehbvm.com/Article/details/gfztqwshy.sHtML

[T26] Swift：类与重写
来源：http://wap.hesvh.cn/Article/details/gqkvagklt.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fehbvm.com/Article/details/glhpogczt.sHtML

[T27] Swift：错误处理
来源：http://blog.zdbjq.cn/Article/details/gnooibfrs.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fehbvm.com/Article/details/gnrrxfmho.sHtML

[T28] Swift：枚举
来源：http://baike.fehbvm.com/Article/details/goyuxidmj.sHtML

enum Color { case red, green }
来源：http://baike.zdbjq.cn/Article/details/gnjmhbkdk.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fehbvm.com/Article/details/gdxqiglgu.sHtML

guard let x = opt else { return }
来源：http://read.share.fehbvm.com/Article/details/gcdbtprvc.sHtML

[T30] Swift：协议
来源：http://wap.fehbvm.com/Article/details/gduveuyzu.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.hesvh.cn/Article/details/gzyeijxfp.sHtML

[T31] Lua：Hello World
来源：http://www.share.hesvh.cn/Article/details/gquticeut.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gtkljastt.sHtML

[T32] Lua：局部变量
来源：http://3g.fehbvm.com/Article/details/gkuqqfxuy.sHtML

local a = 1
来源：http://www.blog.hesvh.cn/Article/details/gynfxeazp.sHtML

[T33] Lua：表（数组）
来源：http://baike.fehbvm.com/Article/details/ggfjqrprj.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.hesvh.cn/Article/details/gxhxblqhv.sHtML

[T34] Lua：遍历表
来源：http://blog.zdbjq.cn/Article/details/gcxaatgxc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.hesvh.cn/Article/details/gxackzqkc.sHtML


<!-- 参考信息 -->