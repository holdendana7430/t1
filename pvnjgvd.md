代发 wailian999

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/gafotoayq.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/gfmrbrgbx.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/gmpqnztth.sHtML

[R29] 定义函数
来源：http://www.share.fehbvm.com/Article/details/ghcoivahq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.hesvh.cn/Article/details/gxvjkqsut.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fehbvm.com/Article/details/gidrepcnc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.hesvh.cn/Article/details/gmtdwrkee.sHtML

[R31] 局部变量
来源：http://read.share.zdbjq.cn/Article/details/gjnxhkypr.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.hesvh.cn/Article/details/grieknliw.sHtML

[R32] 参数个数校验
来源：http://m.share.hesvh.cn/Article/details/gunxrzcnl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gbvlfxwto.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/glgwddnrv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fehbvm.com/Article/details/gponjhhff.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/ggkhdqvxy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gwggkeoec.sHtML

[R35] 后台执行并等待
来源：http://blog.zdbjq.cn/Article/details/gwypttqkk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.zdbjq.cn/Article/details/gorbtxckl.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/ggauhmftz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.hesvh.cn/Article/details/gpjwpoqrd.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.zdbjq.cn/Article/details/gyyuxdgqr.sHtML

files=$(ls -1)
来源：http://3g.hesvh.cn/Article/details/gflbyivxv.sHtML

[R38] 管道串联
来源：http://baike.fehbvm.com/Article/details/gbracbjxh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.hesvh.cn/Article/details/ghyqaqvvx.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/gnacwidzo.sHtML

cmd > out.log 2>&1
来源：http://blog.zdbjq.cn/Article/details/glaqarmqv.sHtML

[R40] 追加写日志
来源：http://wap.fehbvm.com/Article/details/guvhchkmi.sHtML

echo "log" >> out.log
来源：http://wap.fehbvm.com/Article/details/gffbnzjiw.sHtML

[R41] 丢弃输出
来源：http://baike.fehbvm.com/Article/details/guosonlyi.sHtML

cmd >/dev/null 2>&1
来源：http://wap.hesvh.cn/Article/details/gsjhtgbkl.sHtML

[R42] 输入重定向
来源：http://wap.zdbjq.cn/Article/details/ghldwfgnh.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/gbyittpxo.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.zdbjq.cn/Article/details/goqaoksxf.sHtML

find . -name "*.log" -type f
来源：http://blog.zdbjq.cn/Article/details/gmlzombuc.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/gfqbyvyuk.sHtML

find . -mtime -7 -type f
来源：http://m.share.fehbvm.com/Article/details/gnesrlmeg.sHtML

[R45] 批量删除
来源：http://blog.fehbvm.com/Article/details/ggrudwvlz.sHtML

find . -name "*.tmp" -delete
来源：http://baike.zdbjq.cn/Article/details/gfesrwqas.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fehbvm.com/Article/details/gftxddaug.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.zdbjq.cn/Article/details/gxoxmifzk.sHtML

[R47] sed 单行替换
来源：http://www.share.fehbvm.com/Article/details/gaammjuog.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fehbvm.com/Article/details/gisdbrlzv.sHtML

[R48] awk 取指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gziogmjgl.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fehbvm.com/Article/details/gbvldmqwa.sHtML

[R49] awk 带条件
来源：http://www.m.share.fehbvm.com/Article/details/gbmitoxxj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.hesvh.cn/Article/details/grjpkzekx.sHtML

[R50] awk 求和
来源：http://3g.fehbvm.com/Article/details/gyixpjish.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fehbvm.com/Article/details/gfnzjoieq.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/gushghlbd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.zdbjq.cn/Article/details/gzageiyyw.sHtML

[R52] 统计行数
来源：http://baike.fehbvm.com/Article/details/gzfprjqht.sHtML

wc -l a.txt
来源：http://mobile.zdbjq.cn/Article/details/gjarhnrot.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.zdbjq.cn/Article/details/gxtgpxvyr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/goajcsvby.sHtML

[R54] 比较两个文件
来源：http://m.share.fehbvm.com/Article/details/gounubgmr.sHtML

diff a.txt b.txt
来源：http://www.m.share.hesvh.cn/Article/details/gjqnrploz.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/gyxnqltze.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.zdbjq.cn/Article/details/gunefnnhz.sHtML

[R56] 远程拷贝
来源：http://3g.zdbjq.cn/Article/details/gvlgcimvv.sHtML

scp file user@host:/path/
来源：http://www.blog.fehbvm.com/Article/details/gwqznnasn.sHtML

[R57] 远程执行命令
来源：http://www.blog.fehbvm.com/Article/details/gkhgnqcgc.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/gcqxcqkxz.sHtML

[R58] 下载文件
来源：http://wap.zdbjq.cn/Article/details/gwbohefwn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.zdbjq.cn/Article/details/gyffqaomn.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gudmaiyyd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fehbvm.com/Article/details/gdygbunpd.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gjtviyobb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fehbvm.com/Article/details/gdhfzschy.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/gsttnugvo.sHtML

df -h;  du -sh *
来源：http://blog.zdbjq.cn/Article/details/ghfsrudrc.sHtML

[R62] 找最占空间的文件
来源：http://www.share.zdbjq.cn/Article/details/gmlqcqrti.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/gcuvfzvjk.sHtML

[R63] 内存与进程
来源：http://blog.hesvh.cn/Article/details/gisesjred.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fehbvm.com/Article/details/ggzemiubm.sHtML

[R64] 结束进程
来源：http://www.blog.zdbjq.cn/Article/details/gnmqbugrf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.hesvh.cn/Article/details/gcylazlbn.sHtML

[R65] 查看端口占用
来源：http://m.share.zdbjq.cn/Article/details/gmatmsczv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.hesvh.cn/Article/details/gpfbruhlh.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gojtienev.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gxrckhxud.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.zdbjq.cn/Article/details/gvvpcmgyd.sHtML

openssl rand -hex 16
来源：http://m.share.zdbjq.cn/Article/details/gxmkclyft.sHtML

[R68] 计算文件校验值
来源：http://wap.zdbjq.cn/Article/details/gzfgrtxga.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gvirqditl.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/gzipceqks.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/gaqgvbiji.sHtML

[R70] 时间戳与互转
来源：http://www.share.hesvh.cn/Article/details/gheqdfnxo.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fehbvm.com/Article/details/godfbhlvq.sHtML

[R71] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gixqgbpcg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/gbdzxspuj.sHtML

[R72] 等待端口就绪
来源：http://read.share.fehbvm.com/Article/details/gecdedwkv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/ggiitcmzc.sHtML

[R73] 分割大日志
来源：http://www.m.share.fehbvm.com/Article/details/ghxjwckwa.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.hesvh.cn/Article/details/gvrwxdgrj.sHtML

[R74] 批量重命名
来源：http://baike.zdbjq.cn/Article/details/gjgusuxaz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.zdbjq.cn/Article/details/gjqsfjivx.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gutppwpmu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fehbvm.com/Article/details/gdwqwvfpf.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/gebmenody.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gblqiplrs.sHtML

[R77] 读取用户输入
来源：http://www.blog.fehbvm.com/Article/details/gcwegbyzs.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/guodvlbyf.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/gabqzjbhi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/ghaqkverp.sHtML

[R79] 解析命令行选项
来源：http://wap.zdbjq.cn/Article/details/grbnlnppf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/gaiipwdqt.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/gtibhxlxh.sHtML

time ./run.sh
来源：http://www.blog.hesvh.cn/Article/details/gzzvptayr.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfkyeanmz.sHtML

S. C / C++ 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gserpgyrt.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gtrkerkcu.sHtML

[S01] C：Hello World
来源：http://baike.zdbjq.cn/Article/details/gnuleflja.sHtML

#include <stdio.h>
来源：http://wap.hesvh.cn/Article/details/gxxkfkzpg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gkdlvnana.sHtML

[S02] C：变量与格式化输出
来源：http://3g.zdbjq.cn/Article/details/gnzkuijls.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/gioxteacg.sHtML

[S03] C：读入整数
来源：http://3g.fehbvm.com/Article/details/ghsarkmcg.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/gmojugvty.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/gqvhkbkcz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.hesvh.cn/Article/details/gosbulbwo.sHtML

[S05] C：字符串长度
来源：http://read.share.hesvh.cn/Article/details/gyqwsjsgq.sHtML

strlen(s)
来源：http://m.share.zdbjq.cn/Article/details/gxedjjhni.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/gemcrxikj.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/gwuwbvbcy.sHtML

[S07] C：数组遍历求和
来源：http://wap.zdbjq.cn/Article/details/gfxfncvps.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.hesvh.cn/Article/details/gccgdikrq.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fehbvm.com/Article/details/gdpnhidmj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/gitclgfzg.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.hesvh.cn/Article/details/gyqlpcfco.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fehbvm.com/Article/details/gdjbqmhbj.sHtML

[S10] C：指针与解引用
来源：http://mobile.fehbvm.com/Article/details/gmomvssdr.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fehbvm.com/Article/details/gcogvgpbl.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gwohjrsmq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fehbvm.com/Article/details/goremnvds.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gurjjkjov.sHtML

fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gzpfeoslc.sHtML

[S12] C：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gzjwcuzdq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/guxyxscjx.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/gcihzyitt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.hesvh.cn/Article/details/gyhsjojiu.sHtML

[S14] C：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gfsuhgvgf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/gxcqwthhe.sHtML

[S15] C：类型转换
来源：http://wap.hesvh.cn/Article/details/gcmfqlaak.sHtML

(double) a / b
来源：http://3g.zdbjq.cn/Article/details/gbmxkaszl.sHtML

[S16] C：位操作置位
来源：http://3g.zdbjq.cn/Article/details/gevpsltdq.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gbmgtowfw.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gycfrgdgw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.zdbjq.cn/Article/details/getoolkzm.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/gkvjetdpa.sHtML

int main(int argc, char **argv)
来源：http://blog.fehbvm.com/Article/details/gitsriipk.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/gticsoism.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gpjtfcfuz.sHtML

[S20] C：二分查找
来源：http://baike.hesvh.cn/Article/details/ganbuusxn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gujqofkxb.sHtML

[S21] C：字符类别判断
来源：http://www.share.hesvh.cn/Article/details/gxunpmook.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/geylungvq.sHtML

[S22] C：字符串转数字
来源：http://3g.fehbvm.com/Article/details/gogmxfaen.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fehbvm.com/Article/details/ghwxidqaz.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/grxloongn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fehbvm.com/Article/details/grjplawzr.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/gpmstcstu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.zdbjq.cn/Article/details/gjpcsnsgx.sHtML

[S25] C：内存拷贝
来源：http://read.share.fehbvm.com/Article/details/gtobhlspm.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gyaqqoegn.sHtML

[S26] C：内存清零
来源：http://www.share.fehbvm.com/Article/details/gggnuzxqa.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/gvqoesfqz.sHtML

[S27] C：定义常量
来源：http://wap.fehbvm.com/Article/details/gvszlucte.sHtML

const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gduwhfhwk.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/gmzquxcln.sHtML

static int counter = 0;
来源：http://3g.hesvh.cn/Article/details/gtryliuqd.sHtML

[S29] C：变参函数
来源：http://3g.hesvh.cn/Article/details/gyskvroxm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.zdbjq.cn/Article/details/gkwzmpvbk.sHtML

[S30] C：头文件保护
来源：http://3g.fehbvm.com/Article/details/gcopjiwdt.sHtML

#ifndef X_H
来源：http://3g.zdbjq.cn/Article/details/gxlewwqrl.sHtML

#define X_H
来源：http://m.share.zdbjq.cn/Article/details/gwuyaykkz.sHtML

#endif
来源：http://blog.hesvh.cn/Article/details/gzghbmvhp.sHtML

[S31] C++：Hello World
来源：http://3g.hesvh.cn/Article/details/gjqovnlyq.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/gbpawqhik.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fehbvm.com/Article/details/gdfrhvblh.sHtML

[S32] C++：字符串
来源：http://www.m.share.fehbvm.com/Article/details/gyhimtuqv.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.hesvh.cn/Article/details/gxyzjiogx.sHtML

[S33] C++：vector 增删
来源：http://mobile.zdbjq.cn/Article/details/gnhzmsius.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.zdbjq.cn/Article/details/gwqqjoznk.sHtML

[S34] C++：遍历 vector
来源：http://3g.fehbvm.com/Article/details/gczmihuhe.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.hesvh.cn/Article/details/gwrhoqexm.sHtML

[S35] C++：map
来源：http://www.share.fehbvm.com/Article/details/guzbqwwla.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/ggxpldjak.sHtML

[S36] C++：unordered_map
来源：http://www.share.hesvh.cn/Article/details/gndfaqffm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gvxmpwytn.sHtML

[S37] C++：set
来源：http://baike.hesvh.cn/Article/details/gumjqzevf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.hesvh.cn/Article/details/gvcaxvmsu.sHtML

[S38] C++：排序
来源：http://www.m.share.hesvh.cn/Article/details/gzgkamhze.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.hesvh.cn/Article/details/gbtkzbrdh.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fehbvm.com/Article/details/gjfaqdqov.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/gpoffoait.sHtML

[S40] C++：查找元素
来源：http://www.share.hesvh.cn/Article/details/gddaskdzn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.zdbjq.cn/Article/details/glsbojqgj.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gmznyyzbi.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.hesvh.cn/Article/details/gvwvdjvgi.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.zdbjq.cn/Article/details/gfquyzdun.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.zdbjq.cn/Article/details/gpfmngyle.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/gfjlmrffu.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gecuzptpt.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/gekplugeb.sHtML

void inc(int &x) { ++x; }
来源：http://3g.hesvh.cn/Article/details/gvybsteoe.sHtML

[S45] C++：lambda
来源：http://www.share.fehbvm.com/Article/details/gfyzuawqw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.zdbjq.cn/Article/details/gcghzrhcp.sHtML

[S46] C++：函数模板
来源：http://wap.fehbvm.com/Article/details/gnjnrkiqt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.hesvh.cn/Article/details/gonctzklm.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/gtnexfotc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.hesvh.cn/Article/details/gwgfngukl.sHtML

[S48] C++：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/getqjxica.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fehbvm.com/Article/details/gctmxfuby.sHtML

while (std::getline(in, line)) { }
来源：http://3g.zdbjq.cn/Article/details/gjuiqnqxb.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gnrylnaqg.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fehbvm.com/Article/details/gjdihtlhr.sHtML

[S50] C++：格式化数字
来源：http://blog.hesvh.cn/Article/details/gffjxaikc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fehbvm.com/Article/details/gmiecihvi.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/gkurawslv.sHtML

static_cast<double>(a) / b
来源：http://mobile.hesvh.cn/Article/details/gbfgymtjy.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/gqapjetbj.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.zdbjq.cn/Article/details/gjvygkfqe.sHtML

[S53] C++：移动语义
来源：http://www.blog.fehbvm.com/Article/details/gbdokrdes.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.hesvh.cn/Article/details/gyzjbpuxa.sHtML

[S54] C++：异常处理
来源：http://wap.zdbjq.cn/Article/details/gfjrztnzc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fehbvm.com/Article/details/gfiuhvbbn.sHtML

[S55] C++：结构化绑定
来源：http://www.share.zdbjq.cn/Article/details/gibezgbar.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gbuscspiy.sHtML

[S56] C++：optional
来源：http://m.share.hesvh.cn/Article/details/gfihrqwqd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/glgucpwfz.sHtML

[S57] C++：编译期常量
来源：http://www.blog.hesvh.cn/Article/details/ggnmyvfuc.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/gofmsrjrz.sHtML

[S58] C++：命名空间
来源：http://3g.fehbvm.com/Article/details/ggwunrpvm.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.zdbjq.cn/Article/details/gmoahnmdr.sHtML

[S59] C++：静态断言
来源：http://mobile.hesvh.cn/Article/details/gpnfvtqck.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fehbvm.com/Article/details/glizxfvaw.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/gatrgpwza.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fehbvm.com/Article/details/gtoslrqkt.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gsbawjuqy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gbnencrej.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbvcrvwiv.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fehbvm.com/Article/details/geohbrogx.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gnvhezdpr.sHtML

[T02] Kotlin：变量
来源：http://read.share.hesvh.cn/Article/details/gmkatqcdf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.hesvh.cn/Article/details/guthaucnp.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fehbvm.com/Article/details/ggystaeiv.sHtML

"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gympqkllp.sHtML

[T04] Kotlin：空安全
来源：http://read.share.zdbjq.cn/Article/details/gagdallhp.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.hesvh.cn/Article/details/gkqpjxmde.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.hesvh.cn/Article/details/gjddswgtj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fehbvm.com/Article/details/ggpwcunnz.sHtML

[T06] Kotlin：集合映射
来源：http://baike.zdbjq.cn/Article/details/gelmgdtkm.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.hesvh.cn/Article/details/grxstwsin.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.fehbvm.com/Article/details/glwagfleh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/gsfojggwi.sHtML

[T08] Kotlin：数据类
来源：http://m.share.hesvh.cn/Article/details/gtjymhujw.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.zdbjq.cn/Article/details/gztqecrsf.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.hesvh.cn/Article/details/gskytfyob.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fehbvm.com/Article/details/glmzslnnh.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.hesvh.cn/Article/details/gejuzgvcq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.fehbvm.com/Article/details/gvkefzwcs.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fehbvm.com/Article/details/gqqjwfaem.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fehbvm.com/Article/details/gifumwsfr.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fehbvm.com/Article/details/gikyxbdbx.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gqsqnsfei.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fehbvm.com/Article/details/gisyzyrrq.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.zdbjq.cn/Article/details/ghewopbnu.sHtML

[T14] Kotlin：循环
来源：http://blog.zdbjq.cn/Article/details/gyxncrdkd.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gptmtqbxo.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.zdbjq.cn/Article/details/gqmqmonfw.sHtML

interface Shape { fun area(): Double }
来源：http://baike.zdbjq.cn/Article/details/gccizrqlv.sHtML

[T16] Swift：Hello World
来源：http://wap.zdbjq.cn/Article/details/gsraxadxw.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gnjezlqbe.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fehbvm.com/Article/details/giehaijad.sHtML

var a = 1;  let b = 2
来源：http://3g.hesvh.cn/Article/details/gfyymqzge.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gcrztpzvi.sHtML

"值: \(b)"
来源：http://wap.zdbjq.cn/Article/details/gmtevyorq.sHtML

[T19] Swift：可选绑定
来源：http://m.share.zdbjq.cn/Article/details/gseceuwkb.sHtML

if let n = opt { print(n) }
来源：http://blog.zdbjq.cn/Article/details/glrgvstro.sHtML

[T20] Swift：数组操作
来源：http://blog.hesvh.cn/Article/details/gopqrfhge.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fehbvm.com/Article/details/gyelsdukg.sHtML

[T21] Swift：遍历
来源：http://www.blog.fehbvm.com/Article/details/goruswiaf.sHtML

for x in a { print(x) }
来源：http://blog.hesvh.cn/Article/details/gnmjwvauy.sHtML

[T22] Swift：字典
来源：http://m.share.zdbjq.cn/Article/details/gxwxbyibv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fehbvm.com/Article/details/gvljhrlcn.sHtML

[T23] Swift：函数
来源：http://m.share.hesvh.cn/Article/details/gqkqqolne.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fehbvm.com/Article/details/gvcvxbpja.sHtML

[T24] Swift：闭包
来源：http://baike.hesvh.cn/Article/details/gpjftpfrx.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gjuxnwxsj.sHtML

[T25] Swift：结构体
来源：http://wap.fehbvm.com/Article/details/gmkemnlxp.sHtML

struct P { var x: Int }
来源：http://m.share.fehbvm.com/Article/details/gfgbqqvid.sHtML

[T26] Swift：类与重写
来源：http://blog.zdbjq.cn/Article/details/gayywqqib.sHtML

class A: Base { override func f() {} }
来源：http://wap.zdbjq.cn/Article/details/gqdkioiau.sHtML

[T27] Swift：错误处理
来源：http://blog.fehbvm.com/Article/details/gfmnuqdoh.sHtML

do { try f() } catch { print(error) }
来源：http://wap.zdbjq.cn/Article/details/gyrydauqn.sHtML

[T28] Swift：枚举
来源：http://baike.zdbjq.cn/Article/details/gvyqbxtln.sHtML

enum Color { case red, green }
来源：http://wap.fehbvm.com/Article/details/glxtjlwpj.sHtML

[T29] Swift：guard 提前返回
来源：http://m.share.hesvh.cn/Article/details/gypvasind.sHtML

guard let x = opt else { return }
来源：http://wap.fehbvm.com/Article/details/gjlddmxry.sHtML

[T30] Swift：协议
来源：http://wap.hesvh.cn/Article/details/grfsfahcd.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.hesvh.cn/Article/details/gteouoqbe.sHtML


<!-- 参考信息 -->