代发 wailian999

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/gpjplpxws.sHtML

[R28] 浮点运算
来源：http://blog.zdbjq.cn/Article/details/gmhstjtmb.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.zdbjq.cn/Article/details/gnsdshbsc.sHtML

[R29] 定义函数
来源：http://m.share.zdbjq.cn/Article/details/gaufjtuya.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/gtdliybat.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/gdzpxgfet.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.zdbjq.cn/Article/details/gqvvuelbm.sHtML

[R31] 局部变量
来源：http://m.share.hesvh.cn/Article/details/gadcealmx.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.zdbjq.cn/Article/details/gtsdbpxug.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/gahvffhco.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/grgdjfcij.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.zdbjq.cn/Article/details/glyokmmnf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fehbvm.com/Article/details/giqmuevcq.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/gkofrrenm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gngzdqbiw.sHtML

[R35] 后台执行并等待
来源：http://m.share.fehbvm.com/Article/details/gnfqqoian.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/gpvydsgtd.sHtML

[R36] 并发执行多个任务
来源：http://blog.fehbvm.com/Article/details/gtgyigomz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/gdkkogfoo.sHtML

[R37] 把输出赋给变量
来源：http://www.share.hesvh.cn/Article/details/guhjyikyg.sHtML

files=$(ls -1)
来源：http://baike.hesvh.cn/Article/details/grxtctvwf.sHtML

[R38] 管道串联
来源：http://www.share.hesvh.cn/Article/details/gkolgpicq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.hesvh.cn/Article/details/gmwkhudzj.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/gbymetjnl.sHtML

cmd > out.log 2>&1
来源：http://read.share.fehbvm.com/Article/details/gxhbziaze.sHtML

[R40] 追加写日志
来源：http://mobile.zdbjq.cn/Article/details/grdzgavhn.sHtML

echo "log" >> out.log
来源：http://wap.hesvh.cn/Article/details/gcjoklwad.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/gpkmzuovb.sHtML

cmd >/dev/null 2>&1
来源：http://3g.hesvh.cn/Article/details/gznhfiwyk.sHtML

[R42] 输入重定向
来源：http://m.share.zdbjq.cn/Article/details/gwqcukmdq.sHtML

wc -l < a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gcwkikjom.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/gagqyfkxl.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gyzsqhill.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/gczhdqfil.sHtML

find . -mtime -7 -type f
来源：http://mobile.hesvh.cn/Article/details/glqbxitrd.sHtML

[R45] 批量删除
来源：http://www.m.share.fehbvm.com/Article/details/gbjmyggku.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/gosjlcolq.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/gsmzbngrg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fehbvm.com/Article/details/gsjhqodbl.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/gwytvhisf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fehbvm.com/Article/details/gevbpfmbg.sHtML

[R48] awk 取指定列
来源：http://www.share.fehbvm.com/Article/details/gcxjobxmu.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gaqhrflzx.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/gmizgckix.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fehbvm.com/Article/details/gqundnjqa.sHtML

[R50] awk 求和
来源：http://baike.hesvh.cn/Article/details/grknlaqez.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.hesvh.cn/Article/details/guvsnffil.sHtML

[R51] 排序去重取前几
来源：http://read.share.fehbvm.com/Article/details/gbycrbmbw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/gfoiymkkg.sHtML

[R52] 统计行数
来源：http://baike.zdbjq.cn/Article/details/gcrmrlmgt.sHtML

wc -l a.txt
来源：http://3g.fehbvm.com/Article/details/gkhpchdmr.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fehbvm.com/Article/details/ggkneeeao.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fehbvm.com/Article/details/gallrzqjm.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/gskxgqabs.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/gjbzwzfze.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/gvcuocgky.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fehbvm.com/Article/details/ggabxcouj.sHtML

[R56] 远程拷贝
来源：http://blog.hesvh.cn/Article/details/guqtcrldq.sHtML

scp file user@host:/path/
来源：http://mobile.hesvh.cn/Article/details/guwilujmz.sHtML

[R57] 远程执行命令
来源：http://m.share.hesvh.cn/Article/details/gybrlrxus.sHtML

ssh user@host 'uptime'
来源：http://www.share.zdbjq.cn/Article/details/gdxluovhc.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/giuehsira.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/gxfvmuqwo.sHtML

[R59] 发 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gbrwqdksl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.zdbjq.cn/Article/details/ggmypipcq.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gyqcaemax.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.zdbjq.cn/Article/details/gnbvnveod.sHtML

[R61] 磁盘占用
来源：http://wap.zdbjq.cn/Article/details/glfvycvvu.sHtML

df -h;  du -sh *
来源：http://www.blog.zdbjq.cn/Article/details/gdojnfkxm.sHtML

[R62] 找最占空间的文件
来源：http://mobile.hesvh.cn/Article/details/gjcagzxua.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.hesvh.cn/Article/details/gbakvseyb.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/gfmywoaig.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.zdbjq.cn/Article/details/geeqknnij.sHtML

[R64] 结束进程
来源：http://mobile.zdbjq.cn/Article/details/gsyjjgqfr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.zdbjq.cn/Article/details/gsjbbykio.sHtML

[R65] 查看端口占用
来源：http://wap.hesvh.cn/Article/details/gkljsbhbv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.zdbjq.cn/Article/details/gpxpwztih.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/gpvizyfcl.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/ggimweaan.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fehbvm.com/Article/details/gfjconfzs.sHtML

openssl rand -hex 16
来源：http://wap.fehbvm.com/Article/details/gcckjbltv.sHtML

[R68] 计算文件校验值
来源：http://m.share.zdbjq.cn/Article/details/gvlpawnsw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/gbytfswlw.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/gkevojfiw.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/girikyqpa.sHtML

[R70] 时间戳与互转
来源：http://mobile.fehbvm.com/Article/details/gtxtlujdy.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/guldbrzxc.sHtML

[R71] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gsqxkqomr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fehbvm.com/Article/details/glpmxzupu.sHtML

[R72] 等待端口就绪
来源：http://baike.zdbjq.cn/Article/details/gkvkkxlzg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/grjbcouni.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/geltplxqv.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/gtuadpmkc.sHtML

[R74] 批量重命名
来源：http://wap.hesvh.cn/Article/details/gqlejbrzb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.hesvh.cn/Article/details/gexnylvhu.sHtML

[R75] 导出环境变量
来源：http://www.share.zdbjq.cn/Article/details/gkaywfarz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.zdbjq.cn/Article/details/gtdmwufnl.sHtML

[R76] 使用临时文件
来源：http://baike.zdbjq.cn/Article/details/gwzrcehcp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/glvtwvwel.sHtML

[R77] 读取用户输入
来源：http://blog.fehbvm.com/Article/details/gfzqvhwwk.sHtML

read -rp "请输入: " ans
来源：http://3g.zdbjq.cn/Article/details/gqckewvzl.sHtML

[R78] 交互式菜单
来源：http://3g.hesvh.cn/Article/details/guoojiagg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/gngdxeoxl.sHtML

[R79] 解析命令行选项
来源：http://baike.zdbjq.cn/Article/details/gyjgxzemd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.hesvh.cn/Article/details/gaqzqqlrs.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.hesvh.cn/Article/details/gwalvibui.sHtML

time ./run.sh
来源：http://read.share.fehbvm.com/Article/details/gmxignmvg.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gyymhiogj.sHtML

S. C / C++ 专题
来源：http://www.share.zdbjq.cn/Article/details/gggnimiad.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpmhksycm.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gazahovjh.sHtML

#include <stdio.h>
来源：http://read.share.fehbvm.com/Article/details/gppcaapfj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.zdbjq.cn/Article/details/gjswteigj.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fehbvm.com/Article/details/gtaoubavj.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/garinghlf.sHtML

[S03] C：读入整数
来源：http://m.share.zdbjq.cn/Article/details/glzanbskm.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/glndhxhzb.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/gcuowzggr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fehbvm.com/Article/details/gihisehdk.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/ggxhqzixk.sHtML

strlen(s)
来源：http://www.share.zdbjq.cn/Article/details/gubdjdfpv.sHtML

[S06] C：字符串比较
来源：http://read.share.fehbvm.com/Article/details/gkybftbxt.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/gzeundarf.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/gpahmnxyq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.zdbjq.cn/Article/details/geytkjkfm.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.zdbjq.cn/Article/details/gycnpupyl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/gnbwbhzlz.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/ggdbnvxuq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/gytpyfldl.sHtML

[S10] C：指针与解引用
来源：http://blog.zdbjq.cn/Article/details/gnilqbvlq.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/gziaebcmk.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gjqbfldbs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/gpjynukpq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.zdbjq.cn/Article/details/gvvqmdicw.sHtML

fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gegranbti.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/ghnhjfnoy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gkqldjsyf.sHtML

[S13] C：宏定义
来源：http://baike.fehbvm.com/Article/details/gbgiasxys.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/gqodacfdk.sHtML

[S14] C：枚举
来源：http://mobile.fehbvm.com/Article/details/ghiovrwpd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.hesvh.cn/Article/details/gyvvtqbww.sHtML

[S15] C：类型转换
来源：http://blog.hesvh.cn/Article/details/ggzsrzdrw.sHtML

(double) a / b
来源：http://blog.fehbvm.com/Article/details/ghicqveew.sHtML

[S16] C：位操作置位
来源：http://www.share.fehbvm.com/Article/details/grpbnjted.sHtML

x |= (1 << 3);
来源：http://www.share.fehbvm.com/Article/details/gifvgziyj.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fehbvm.com/Article/details/gnhokttlr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.hesvh.cn/Article/details/gaqltusyh.sHtML

[S18] C：命令行参数
来源：http://m.share.hesvh.cn/Article/details/gldbvpwoy.sHtML

int main(int argc, char **argv)
来源：http://3g.zdbjq.cn/Article/details/gnafhmvtd.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/ghyjgyufy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gcxdgihnc.sHtML

[S20] C：二分查找
来源：http://m.share.fehbvm.com/Article/details/gzdpdqlem.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gxalgpsbj.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/gqrtxakvd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fehbvm.com/Article/details/goswzewcb.sHtML

[S22] C：字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/gcocrwcls.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.zdbjq.cn/Article/details/gspugdnur.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/gsforlhsp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.hesvh.cn/Article/details/grkinnjep.sHtML

[S24] C：获取本地时间
来源：http://www.blog.hesvh.cn/Article/details/gvmmplrox.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.hesvh.cn/Article/details/gpjavnitu.sHtML

[S25] C：内存拷贝
来源：http://baike.hesvh.cn/Article/details/gthtxkpbh.sHtML

memcpy(dst, src, n);
来源：http://mobile.zdbjq.cn/Article/details/gyktulqed.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/gxarrmqkf.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/gurxenmgr.sHtML

[S27] C：定义常量
来源：http://www.m.share.hesvh.cn/Article/details/gpgsgxzas.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gltbkrsyt.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/gspoinbpk.sHtML

static int counter = 0;
来源：http://3g.fehbvm.com/Article/details/guhbnxwcs.sHtML

[S29] C：变参函数
来源：http://www.share.fehbvm.com/Article/details/gzrihaptf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.zdbjq.cn/Article/details/gndnkcjms.sHtML

[S30] C：头文件保护
来源：http://read.share.zdbjq.cn/Article/details/gasjjxeyw.sHtML

#ifndef X_H
来源：http://www.blog.fehbvm.com/Article/details/gqcfglpjb.sHtML

#define X_H
来源：http://www.m.share.hesvh.cn/Article/details/gdqwwwyxr.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/gjxbdxqwk.sHtML

[S31] C++：Hello World
来源：http://m.share.hesvh.cn/Article/details/gkmcorrhb.sHtML

#include <iostream>
来源：http://read.share.fehbvm.com/Article/details/guoviabfo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fehbvm.com/Article/details/gkdsxcihp.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/gmvfmoirr.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/gicfbeuey.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/gnukfxmez.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.zdbjq.cn/Article/details/gatxaduib.sHtML

[S34] C++：遍历 vector
来源：http://3g.hesvh.cn/Article/details/ghbohkswa.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fehbvm.com/Article/details/gctsykpzf.sHtML

[S35] C++：map
来源：http://read.share.zdbjq.cn/Article/details/gvghkoola.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/grsbtkrrd.sHtML

[S36] C++：unordered_map
来源：http://www.blog.hesvh.cn/Article/details/gabweajdy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/goygxiqgx.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/gxncvnrnq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.zdbjq.cn/Article/details/gqtfiomkw.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/grfzfotns.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.zdbjq.cn/Article/details/gyniebdxv.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/gscaagpye.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fehbvm.com/Article/details/gmluhytgv.sHtML

[S40] C++：查找元素
来源：http://wap.zdbjq.cn/Article/details/gkmommqcc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gbecmmceo.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/gaiokbuqp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/gyqwbyazg.sHtML

[S42] C++：继承与虚函数
来源：http://wap.hesvh.cn/Article/details/gjwpgfeuy.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/glbvkisml.sHtML

[S43] C++：智能指针
来源：http://blog.fehbvm.com/Article/details/gitdpqyzx.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.hesvh.cn/Article/details/gpxnfhmxg.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gfefbtbwq.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.hesvh.cn/Article/details/gsadpnkcf.sHtML

[S45] C++：lambda
来源：http://mobile.fehbvm.com/Article/details/gpiyofgua.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fehbvm.com/Article/details/gigoywqyn.sHtML

[S46] C++：函数模板
来源：http://blog.zdbjq.cn/Article/details/godlbevrd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.zdbjq.cn/Article/details/gasnyuhhm.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fehbvm.com/Article/details/gtthigozq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/gsshwclqd.sHtML

[S48] C++：逐行读文件
来源：http://wap.fehbvm.com/Article/details/giyyjamuv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.zdbjq.cn/Article/details/gayskywmt.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/gdhsdrgpy.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/gsixdmwbs.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.hesvh.cn/Article/details/gzyugiemi.sHtML

[S50] C++：格式化数字
来源：http://blog.fehbvm.com/Article/details/ggpjokakb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/ggdvfgary.sHtML

[S51] C++：显式类型转换
来源：http://blog.zdbjq.cn/Article/details/gbbljjzou.sHtML

static_cast<double>(a) / b
来源：http://m.share.hesvh.cn/Article/details/gcnrtbvte.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.zdbjq.cn/Article/details/gqfklrjeu.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fehbvm.com/Article/details/gwmqwgzqg.sHtML

[S53] C++：移动语义
来源：http://3g.zdbjq.cn/Article/details/gyidsxntj.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.zdbjq.cn/Article/details/gjrhcnfwc.sHtML

[S54] C++：异常处理
来源：http://blog.fehbvm.com/Article/details/gjztyusov.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fehbvm.com/Article/details/gladtjzqn.sHtML

[S55] C++：结构化绑定
来源：http://3g.zdbjq.cn/Article/details/ggkpzljsa.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.hesvh.cn/Article/details/ggtqnwbhi.sHtML

[S56] C++：optional
来源：http://blog.hesvh.cn/Article/details/gathlesmo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.hesvh.cn/Article/details/gkricvlhy.sHtML

[S57] C++：编译期常量
来源：http://3g.fehbvm.com/Article/details/gqmalqywj.sHtML

constexpr int N = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gnioiecdj.sHtML

[S58] C++：命名空间
来源：http://www.m.share.hesvh.cn/Article/details/guivwbuqo.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fehbvm.com/Article/details/gjqbscqbq.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/gdattjydv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.zdbjq.cn/Article/details/gilyhgalz.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/ghdxxjbpi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.hesvh.cn/Article/details/gfgxtijbx.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gobznlfej.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gqfdpbxhn.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwnybbqwl.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fehbvm.com/Article/details/gzksihtbb.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gmeguatzh.sHtML

[T02] Kotlin：变量
来源：http://mobile.hesvh.cn/Article/details/gluknwlej.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.hesvh.cn/Article/details/gualwcqiy.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fehbvm.com/Article/details/gaahxwwmn.sHtML

"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gfzmwqfhl.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/gkkdzxyuc.sHtML

val n: String? = null;  n?.length
来源：http://baike.hesvh.cn/Article/details/gcqwlwwqf.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gxzsntpuz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.hesvh.cn/Article/details/gkuiwlwch.sHtML

[T06] Kotlin：集合映射
来源：http://wap.zdbjq.cn/Article/details/gtldimtjo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.zdbjq.cn/Article/details/gxwbyfoef.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gmcyuqndh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fehbvm.com/Article/details/gbtivnwua.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fehbvm.com/Article/details/gdoyymlpr.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gczllohnc.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.zdbjq.cn/Article/details/glixhnptr.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.hesvh.cn/Article/details/gnwghykha.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/goiqflhmq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.hesvh.cn/Article/details/ggshoteyg.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.zdbjq.cn/Article/details/gqxhykjrz.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/guxwrwhqp.sHtML

[T12] Kotlin：解构声明
来源：http://blog.zdbjq.cn/Article/details/ghsatfboh.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gqnpazcqo.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.zdbjq.cn/Article/details/gfgekouyy.sHtML

val m = mapOf("a" to 1)
来源：http://blog.hesvh.cn/Article/details/gazbreymp.sHtML

[T14] Kotlin：循环
来源：http://mobile.hesvh.cn/Article/details/gbpgzfrdl.sHtML

for (i in 1..10) println(i)
来源：http://3g.hesvh.cn/Article/details/gpyuzessl.sHtML

[T15] Kotlin：接口
来源：http://read.share.hesvh.cn/Article/details/gvudsydjh.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.hesvh.cn/Article/details/gfxjmobrs.sHtML

[T16] Swift：Hello World
来源：http://wap.hesvh.cn/Article/details/gyajpelwa.sHtML

print("Hello")
来源：http://mobile.fehbvm.com/Article/details/gsdrvunkg.sHtML

[T17] Swift：变量与常量
来源：http://baike.fehbvm.com/Article/details/gaizywzir.sHtML

var a = 1;  let b = 2
来源：http://www.share.fehbvm.com/Article/details/grnchtano.sHtML

[T18] Swift：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/ggionzmxj.sHtML

"值: \(b)"
来源：http://www.share.zdbjq.cn/Article/details/gzfcwmmqo.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.zdbjq.cn/Article/details/gjxzdqffm.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/gaskirqnz.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.hesvh.cn/Article/details/gztrsczjq.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.hesvh.cn/Article/details/gqrefunig.sHtML

[T21] Swift：遍历
来源：http://www.share.hesvh.cn/Article/details/gxxgbdvya.sHtML

for x in a { print(x) }
来源：http://3g.hesvh.cn/Article/details/gyiprzvoe.sHtML

[T22] Swift：字典
来源：http://mobile.zdbjq.cn/Article/details/gztvmmwvl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.hesvh.cn/Article/details/gjfpqickx.sHtML

[T23] Swift：函数
来源：http://wap.hesvh.cn/Article/details/gxjdlejnd.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/gapjsvyoi.sHtML

[T24] Swift：闭包
来源：http://read.share.hesvh.cn/Article/details/geeriofpo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/ggluuneym.sHtML

[T25] Swift：结构体
来源：http://m.share.hesvh.cn/Article/details/ghzdlfiyz.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/gdyvfiavw.sHtML

[T26] Swift：类与重写
来源：http://www.share.fehbvm.com/Article/details/ggfwhqjeb.sHtML

class A: Base { override func f() {} }
来源：http://wap.zdbjq.cn/Article/details/gvnjedbov.sHtML

[T27] Swift：错误处理
来源：http://blog.fehbvm.com/Article/details/gtwnuzvfo.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.hesvh.cn/Article/details/gsceekhye.sHtML

[T28] Swift：枚举
来源：http://m.share.fehbvm.com/Article/details/glemdkpdn.sHtML

enum Color { case red, green }
来源：http://3g.zdbjq.cn/Article/details/ganoguqnw.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.hesvh.cn/Article/details/gzpwamezs.sHtML

guard let x = opt else { return }
来源：http://m.share.hesvh.cn/Article/details/gqjrpujbk.sHtML

[T30] Swift：协议
来源：http://m.share.zdbjq.cn/Article/details/glknzwvfo.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.zdbjq.cn/Article/details/gcimedrsp.sHtML


<!-- 参考信息 -->