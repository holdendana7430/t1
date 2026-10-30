代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/gjjhhixnh.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gxgfbqzyw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/gilyynnyn.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gywwhawzi.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqqbysfu.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzwwpkuh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gsccfojxg.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtqgjzhq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gihjtgsqd.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/glimlpyvb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gjozmigjg.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gvyxabjuo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/gbanxhbjc.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gthvfucim.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdmystfi.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqycmhmdv.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gvqidodwa.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwwzltpz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gtoootbrj.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/gcwgfmmmx.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gojkmdldo.sHtML

[R40] 追加写日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gayccickb.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/glxjddkyh.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gugnwuqjd.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gxmrqqfjd.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojhkwbcy.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gsxfqwnof.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/grcogeazi.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjxacrjm.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gfwemtegz.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrsfmmuz.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gwpigdyli.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gyaubwcpf.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/gdunvpczb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/gklzpmqdw.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gpaczampi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkccwyufa.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gnsmjvjmq.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gcevwepwr.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gbzfcewtd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/grbnqcgvg.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gaibuvuov.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gnnheskdh.sHtML

[R51] 排序去重取前几
来源：http://read.share.fanxiaobao.xyz/Article/details/gdttpnjfe.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsoirtwaj.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/gfvqjdxsv.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gipjudmmp.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/gjjzffjsk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gxksjugsb.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/galdbwfzg.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtavuqpgq.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmieeaom.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gngnflwin.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gcvjhhbxr.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/gsjhirsds.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gzauqkblb.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gnhmhfoeq.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/guqjuaewk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gssaktgfi.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsvhoesc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqloetoxh.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gfqdwvaii.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gfyslgbdi.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gfyxenduz.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfmdhhxn.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gaxlgswli.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzvsqvqk.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjgzppfm.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhhvvihx.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/glaxzfljk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfanfadom.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbnnqbom.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/gjeghfysy.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmayawua.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/gcowyvipf.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geczzqefh.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgazunps.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/gpyotbfyx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gknvsuxkv.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/glrsxyrdg.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gamtxdxfv.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqpdpnxs.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gbcysukmg.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gduwurlqz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/gujdypkss.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqvceyxm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gjzzawcgk.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/grhxnqzvq.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/gsphjsonw.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygeoimyc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gzlffqvrs.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkiwssts.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxxpdgar.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/glpotsvxz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmwysmne.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gnlmsvxcn.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyoykyvfl.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtdgkxve.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctzaubul.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gvgoysshu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdowhbqy.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqvopmqf.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnrfqxcs.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gflbwtszb.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gvpvoaplx.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gkmrromio.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskdakqyl.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjnjdtem.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbjuknpxg.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/ggzplsjni.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gtfykdket.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gtkycfsdo.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhlxzgfx.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlgvatqj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gjoaoxice.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gvypmfakz.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhhrrofo.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/grrsdxztj.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/gwilqgeye.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gshbaligs.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gudeetpdo.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gqwkqflqz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtxkhxut.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/grcpahiqg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gaddhtbhp.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/grriumahu.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gjdhxjtpz.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqqgafkn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gowcrdrsr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/ginvicsns.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gyvzmjzzj.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gbnntqnli.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gbbbzuwbu.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gayzxcief.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gowimdkze.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwyagitw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gognzidqd.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gniiarqmv.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntzhjiih.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/grdmgkkzo.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxkkfrby.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gkqliozvj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gberjmgsk.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/glwarspuh.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkqoznmv.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxnqjhxy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxjsebvi.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gheyavvpa.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gkjhkrhqm.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/glbqrtcft.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/gpqzgzexe.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpptzwbs.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzoguart.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gkzbtxclr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvdijzkh.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gyobavcul.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkuxkmso.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycbvnvld.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/girwvoeac.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/ggltdjulx.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/gujmfhafo.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxknjyzd.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/glbozvpqo.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/grysdwjyk.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpuudscpn.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvtzkywp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmzrunib.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdejmlbt.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/ghckqzfag.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gzwdekuhm.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmeqwmsx.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gmgmrhfcx.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/gtonznkvg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnbagmyov.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbbmowhz.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/goptispew.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gbimbuimx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjwutaai.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/graklhydi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gljrdzlyt.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvuqpwyx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngmpaexb.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrhvhukd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gjndvfzmw.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/ggkwhpvzz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gvzefatox.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/glqmzbnfj.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/godcbgrny.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjvvtgcz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/gxtgnyoro.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/ghgypqkws.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/giqhmjnfc.sHtML

[S41] C++：类与构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/gykfvmjim.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtvnkueq.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gujmlqpou.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/gdoeswhve.sHtML

[S43] C++：智能指针
来源：http://mobile.fanxiaobao.xyz/Article/details/glxacwnmt.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/gkwerbgdz.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfcdtzqi.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gwywftkki.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhtfsonf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllwerubd.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzkhwqfs.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjfgdcidj.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gnqeqbrzq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxkjzymby.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gqgxedesj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/gouvhyyog.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gvrxvwxll.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gownilhfs.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfqcqkkn.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gdbybmxlj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/ghopvpyru.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gkpxporok.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/gqmnftbxv.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/gfejerwxb.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/gcmphtwmd.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/gwvadfolh.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gzwmbgvkj.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geffnhwxu.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbiniapph.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gruphbsuy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspofpjij.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/ggmvzfqwi.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtzxfwsa.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwtebngo.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/giaecbbvt.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfrvfxcr.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gzbmwdnec.sHtML

[S59] C++：静态断言
来源：http://blog.fanxiaobao.xyz/Article/details/gxvapnxve.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/ghrfppfgt.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gxnzeuqaz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcymtrhi.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gymtjbtxy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/gvvqnqiua.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gacwreeyt.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gkofknedn.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdhzplgn.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gtyicrktj.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfslidxg.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvgkxbjw.sHtML

"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gemilrnxb.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/gmvhrhkpz.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gclmgehwv.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbscdumx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvvyecew.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/grzjudpyk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgbgmyor.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqubgwxn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fanxiaobao.xyz/Article/details/gvlbgcsgc.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/grqjpeuni.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/gqqyjfsuf.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fanxiaobao.xyz/Article/details/gvvqaitxf.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.fanxiaobao.xyz/Article/details/glkrrzruv.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjidlatgt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/grfsvvntg.sHtML

[T11] Kotlin：协程
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcwmsvqh.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdytzpbbf.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gauycjmuh.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gskvroptz.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gdanqxeqf.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcisxvpuf.sHtML

[T14] Kotlin：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqdlwqef.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsuveflt.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/ggyxyymcj.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fanxiaobao.xyz/Article/details/gbuflulle.sHtML

[T16] Swift：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gwbrvfqyc.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnejebum.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/glsnvrcov.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/ggzcscbsi.sHtML

[T18] Swift：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gbbobtvcz.sHtML

"值: \(b)"
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvfubjcf.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwshjqeu.sHtML

if let n = opt { print(n) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqzmlabm.sHtML

[T20] Swift：数组操作
来源：http://www.share.fanxiaobao.xyz/Article/details/geysmrqxy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fanxiaobao.xyz/Article/details/gqkgvalsi.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvzrpohw.sHtML

for x in a { print(x) }
来源：http://baike.fanxiaobao.xyz/Article/details/gfjonodek.sHtML

[T22] Swift：字典
来源：http://read.share.fanxiaobao.xyz/Article/details/glrxwvjia.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gkypxqddb.sHtML

[T23] Swift：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gkifocqmr.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwgxlzux.sHtML

[T24] Swift：闭包
来源：http://baike.fanxiaobao.xyz/Article/details/gkmryiadg.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gseicllhi.sHtML

[T25] Swift：结构体
来源：http://read.share.fanxiaobao.xyz/Article/details/gppbvdrlo.sHtML

struct P { var x: Int }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgvlquje.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypffhqdy.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgxhczli.sHtML

[T27] Swift：错误处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gduufkbff.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbyzutvc.sHtML

[T28] Swift：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gwtjuedxl.sHtML

enum Color { case red, green }
来源：http://blog.fanxiaobao.xyz/Article/details/gehhfugkw.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdhyorqz.sHtML

guard let x = opt else { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gwcudecmt.sHtML

[T30] Swift：协议
来源：http://mobile.fanxiaobao.xyz/Article/details/gwylzvljs.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzapdfqs.sHtML

[T31] Lua：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdpwqsap.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfbtdrev.sHtML

[T32] Lua：局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbkdrlaf.sHtML

local a = 1
来源：http://3g.fanxiaobao.xyz/Article/details/gggusuqih.sHtML


<!-- 参考信息 -->