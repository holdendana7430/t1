代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fehbvm.com/Article/details/gjzvnbluc.sHtML

[R30] 函数返回状态码
来源：http://read.share.fehbvm.com/Article/details/ggdrgevtg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/gjkvnqpbx.sHtML

[R31] 局部变量
来源：http://mobile.zdbjq.cn/Article/details/gikxhsicv.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.zdbjq.cn/Article/details/gbbncsfvl.sHtML

[R32] 参数个数校验
来源：http://m.share.hesvh.cn/Article/details/gqralrlvy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gayycedsi.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fehbvm.com/Article/details/gjykomnpr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.hesvh.cn/Article/details/gefbszlbv.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/ghzjfolxs.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gayybhkys.sHtML

[R35] 后台执行并等待
来源：http://3g.fehbvm.com/Article/details/goucbvkla.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fehbvm.com/Article/details/gitstwkbq.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fehbvm.com/Article/details/gxxnaihas.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fehbvm.com/Article/details/gdyvgqsjq.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.hesvh.cn/Article/details/gcjftlrgk.sHtML

files=$(ls -1)
来源：http://www.m.share.hesvh.cn/Article/details/gucqmhbij.sHtML

[R38] 管道串联
来源：http://wap.hesvh.cn/Article/details/gdiwdxbqk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.zdbjq.cn/Article/details/gxbtemzbk.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/gaprzeoau.sHtML

cmd > out.log 2>&1
来源：http://blog.hesvh.cn/Article/details/gzpnwojgz.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/gqxtfkejc.sHtML

echo "log" >> out.log
来源：http://www.m.share.hesvh.cn/Article/details/gqugpzlbg.sHtML

[R41] 丢弃输出
来源：http://wap.hesvh.cn/Article/details/gbrmgewqs.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/gbyznvssv.sHtML

[R42] 输入重定向
来源：http://mobile.hesvh.cn/Article/details/gtxofzaij.sHtML

wc -l < a.txt
来源：http://3g.fehbvm.com/Article/details/gaetscrxf.sHtML

[R43] 按名字查找文件
来源：http://blog.hesvh.cn/Article/details/gepankwqt.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/gfnhghnqw.sHtML

[R44] 按修改时间查找
来源：http://read.share.hesvh.cn/Article/details/gatyahhvl.sHtML

find . -mtime -7 -type f
来源：http://blog.fehbvm.com/Article/details/gamkamuea.sHtML

[R45] 批量删除
来源：http://www.blog.hesvh.cn/Article/details/ghoqigicm.sHtML

find . -name "*.tmp" -delete
来源：http://baike.hesvh.cn/Article/details/gyrfepkgj.sHtML

[R46] 递归替换文件内容
来源：http://wap.zdbjq.cn/Article/details/gttrtxmew.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.zdbjq.cn/Article/details/gcaomezeu.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/glkyriejd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fehbvm.com/Article/details/gwyxjecux.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/gktxblmwy.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gelvmadgk.sHtML

[R49] awk 带条件
来源：http://m.share.fehbvm.com/Article/details/ggxloenhw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/gwujbfvhc.sHtML

[R50] awk 求和
来源：http://blog.fehbvm.com/Article/details/gnmulabgb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gkbcepyca.sHtML

[R51] 排序去重取前几
来源：http://mobile.zdbjq.cn/Article/details/ghvrfbahe.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/glejqfple.sHtML

[R52] 统计行数
来源：http://mobile.hesvh.cn/Article/details/gnteyhypu.sHtML

wc -l a.txt
来源：http://3g.hesvh.cn/Article/details/gnbszblvx.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/gajfrlmup.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.hesvh.cn/Article/details/gjkelandu.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/gigyyvvlg.sHtML

diff a.txt b.txt
来源：http://blog.zdbjq.cn/Article/details/gdqpjbzyk.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/gyukxepus.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.zdbjq.cn/Article/details/gqukofzzn.sHtML

[R56] 远程拷贝
来源：http://m.share.zdbjq.cn/Article/details/gkjjlvoqf.sHtML

scp file user@host:/path/
来源：http://baike.hesvh.cn/Article/details/ggqlhfrbp.sHtML

[R57] 远程执行命令
来源：http://m.share.fehbvm.com/Article/details/gfdytdfne.sHtML

ssh user@host 'uptime'
来源：http://read.share.hesvh.cn/Article/details/gyzppbvxl.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/gxxfxotqc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fehbvm.com/Article/details/gbwalokwi.sHtML

[R59] 发 POST JSON
来源：http://baike.fehbvm.com/Article/details/gmkondajo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.zdbjq.cn/Article/details/gdehwedwo.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gvvtawjdc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/gvxqbselj.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/gzvppolpq.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/gtvvnhbaf.sHtML

[R62] 找最占空间的文件
来源：http://www.share.zdbjq.cn/Article/details/ghrdtlrdb.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/gkvmynywd.sHtML

[R63] 内存与进程
来源：http://www.m.share.zdbjq.cn/Article/details/gucmaqetj.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.hesvh.cn/Article/details/glcyknxga.sHtML

[R64] 结束进程
来源：http://3g.zdbjq.cn/Article/details/gmglxogqq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fehbvm.com/Article/details/glmlnpynh.sHtML

[R65] 查看端口占用
来源：http://blog.hesvh.cn/Article/details/ganoutkom.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fehbvm.com/Article/details/gwcwiyilo.sHtML

[R66] 定时任务
来源：http://wap.fehbvm.com/Article/details/gdktcrzkr.sHtML

crontab -e;  crontab -l
来源：http://baike.hesvh.cn/Article/details/gfciubprb.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.zdbjq.cn/Article/details/gcmymzlqs.sHtML

openssl rand -hex 16
来源：http://mobile.zdbjq.cn/Article/details/gikdsiedp.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/goxoybvkr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fehbvm.com/Article/details/gwofabigw.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fehbvm.com/Article/details/gskqdhusv.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/gnkiopmgn.sHtML

[R70] 时间戳与互转
来源：http://m.share.hesvh.cn/Article/details/gftlbddot.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fehbvm.com/Article/details/gtzakgaeo.sHtML

[R71] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/guwoomqjz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/gebqzakka.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/gbayomhwz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gwubwsmpi.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/gtuijlxxp.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/gudgkvilc.sHtML

[R74] 批量重命名
来源：http://m.share.zdbjq.cn/Article/details/gczjbgcqw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.zdbjq.cn/Article/details/grqcuibyc.sHtML

[R75] 导出环境变量
来源：http://mobile.fehbvm.com/Article/details/glfswwuzm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fehbvm.com/Article/details/gbsdodepx.sHtML

[R76] 使用临时文件
来源：http://3g.hesvh.cn/Article/details/gotuqithe.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gkicdgxdc.sHtML

[R77] 读取用户输入
来源：http://m.share.hesvh.cn/Article/details/giegfrrop.sHtML

read -rp "请输入: " ans
来源：http://baike.fehbvm.com/Article/details/gegavocym.sHtML

[R78] 交互式菜单
来源：http://mobile.zdbjq.cn/Article/details/gtlksriuw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fehbvm.com/Article/details/gcbnzewox.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/goinayrfg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fehbvm.com/Article/details/gekwmyczn.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fehbvm.com/Article/details/golpmtawc.sHtML

time ./run.sh
来源：http://www.m.share.fehbvm.com/Article/details/gwdrfklit.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghgkrmyev.sHtML

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/ghpwejxov.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gcnmektiz.sHtML

[S01] C：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gmvhwzzdc.sHtML

#include <stdio.h>
来源：http://blog.zdbjq.cn/Article/details/ginggccoj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.zdbjq.cn/Article/details/gjdpaokcu.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fehbvm.com/Article/details/gqtbgzglz.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.zdbjq.cn/Article/details/gmaoxvcbw.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gbwvzkogp.sHtML

int x; scanf("%d", &x);
来源：http://wap.hesvh.cn/Article/details/guhbzpcen.sHtML

[S04] C：字符串复制
来源：http://www.blog.fehbvm.com/Article/details/ggwhhpavh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/girjhjmjk.sHtML

[S05] C：字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gidgfwprb.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/giyezvdnz.sHtML

[S06] C：字符串比较
来源：http://3g.fehbvm.com/Article/details/gqpbkduzw.sHtML

strcmp(a, b) == 0
来源：http://3g.fehbvm.com/Article/details/gciovafot.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fehbvm.com/Article/details/gmzxvoawx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.zdbjq.cn/Article/details/gkjkkuxbz.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/gkfanqhjq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/gbbbfnoro.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fehbvm.com/Article/details/gzfdvoccs.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/geafvrzgq.sHtML

[S10] C：指针与解引用
来源：http://m.share.zdbjq.cn/Article/details/gjhnxnjdq.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/gxkrxyxid.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gnnsnafwi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.hesvh.cn/Article/details/gqrynvlzj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.hesvh.cn/Article/details/ggdmnoyaj.sHtML

fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gjmydzwju.sHtML

[S12] C：写文件
来源：http://blog.hesvh.cn/Article/details/gjcymvkhh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gmwgufszr.sHtML

[S13] C：宏定义
来源：http://www.share.fehbvm.com/Article/details/gmgxglbtp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fehbvm.com/Article/details/gevmgfupp.sHtML

[S14] C：枚举
来源：http://www.blog.hesvh.cn/Article/details/gcojtjcyt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fehbvm.com/Article/details/gitsektxc.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/glhajlhut.sHtML

(double) a / b
来源：http://blog.zdbjq.cn/Article/details/gnlgvsmsa.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/gydzpexqo.sHtML

x |= (1 << 3);
来源：http://baike.zdbjq.cn/Article/details/gnlyfxkgn.sHtML

[S17] C：安全拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gviyfixpt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/gzddxfrfn.sHtML

[S18] C：命令行参数
来源：http://www.blog.fehbvm.com/Article/details/gmufoayfs.sHtML

int main(int argc, char **argv)
来源：http://3g.zdbjq.cn/Article/details/gzpoqtogf.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/ghuqpvigt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gdsmopzhi.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/gtdsmxidd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/ggjemvgtv.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/gpeofoxlp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/gwaemhrtr.sHtML

[S22] C：字符串转数字
来源：http://3g.fehbvm.com/Article/details/gxskzqkak.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/gvzbzomuz.sHtML

[S23] C：随机数
来源：http://mobile.hesvh.cn/Article/details/gborhxtfs.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.zdbjq.cn/Article/details/glhfayifr.sHtML

[S24] C：获取本地时间
来源：http://blog.hesvh.cn/Article/details/gszrkmmbz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fehbvm.com/Article/details/gjxwrtkhi.sHtML

[S25] C：内存拷贝
来源：http://m.share.hesvh.cn/Article/details/glzacpopw.sHtML

memcpy(dst, src, n);
来源：http://mobile.zdbjq.cn/Article/details/gcmfyyqbt.sHtML

[S26] C：内存清零
来源：http://mobile.hesvh.cn/Article/details/gyplxcojs.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fehbvm.com/Article/details/gxtchbext.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/gdrmwauxr.sHtML

const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gpyvoitnr.sHtML

[S28] C：静态变量
来源：http://blog.zdbjq.cn/Article/details/gfangrkal.sHtML

static int counter = 0;
来源：http://mobile.fehbvm.com/Article/details/gzlixolwx.sHtML

[S29] C：变参函数
来源：http://www.blog.zdbjq.cn/Article/details/gklrwlpfk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.hesvh.cn/Article/details/ggwbbpycj.sHtML

[S30] C：头文件保护
来源：http://read.share.zdbjq.cn/Article/details/gekzxulkb.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/gbqjhxnym.sHtML

#define X_H
来源：http://3g.zdbjq.cn/Article/details/gnfwyziry.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/gukxufrmv.sHtML

[S31] C++：Hello World
来源：http://blog.zdbjq.cn/Article/details/gvbzunpir.sHtML

#include <iostream>
来源：http://mobile.fehbvm.com/Article/details/ggsjypfcx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.hesvh.cn/Article/details/ggczdqcxc.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gytpiripk.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.hesvh.cn/Article/details/gtuyrkmjf.sHtML

[S33] C++：vector 增删
来源：http://wap.zdbjq.cn/Article/details/gwmstjrdi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.hesvh.cn/Article/details/gulwdvvgf.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fehbvm.com/Article/details/gwdbvtucd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.hesvh.cn/Article/details/gkpampfmn.sHtML

[S35] C++：map
来源：http://www.share.fehbvm.com/Article/details/gpdjiplea.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gootrgcek.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/gqlelsjat.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gczpedfvq.sHtML

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/gtzchsbsx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gltpyjpzz.sHtML

[S38] C++：排序
来源：http://3g.zdbjq.cn/Article/details/gdtvxfbgq.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fehbvm.com/Article/details/gtxjgejno.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/gajglxhxr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.hesvh.cn/Article/details/ghyakxqll.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fehbvm.com/Article/details/gxjnqjwbc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.hesvh.cn/Article/details/gnqyjmsgw.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fehbvm.com/Article/details/gxitejbws.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.hesvh.cn/Article/details/gqlfrkmls.sHtML

[S42] C++：继承与虚函数
来源：http://blog.hesvh.cn/Article/details/gmmccrtlg.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fehbvm.com/Article/details/gqyygpuqc.sHtML

[S43] C++：智能指针
来源：http://baike.fehbvm.com/Article/details/gooudoodq.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.hesvh.cn/Article/details/gayzfguto.sHtML

[S44] C++：引用传参
来源：http://m.share.hesvh.cn/Article/details/gtdaztknb.sHtML

void inc(int &x) { ++x; }
来源：http://blog.hesvh.cn/Article/details/gmkkgwdhi.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/grndgggnt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.hesvh.cn/Article/details/gdokumcid.sHtML

[S46] C++：函数模板
来源：http://m.share.hesvh.cn/Article/details/gmdcvvftk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/gsvfqxiev.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fehbvm.com/Article/details/gedefsckf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.zdbjq.cn/Article/details/gewunzvel.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gcakuimko.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fehbvm.com/Article/details/gaqgxydhd.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/gohphnofj.sHtML

[S49] C++：写文件
来源：http://3g.hesvh.cn/Article/details/gqtxcjabj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.hesvh.cn/Article/details/gxvaikjfp.sHtML

[S50] C++：格式化数字
来源：http://mobile.fehbvm.com/Article/details/gusoytgbi.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gzzdpawea.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gfpyepzye.sHtML

static_cast<double>(a) / b
来源：http://3g.zdbjq.cn/Article/details/ghonlxuvo.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/gldyolhfn.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/gfbjhkiou.sHtML

[S53] C++：移动语义
来源：http://www.blog.fehbvm.com/Article/details/gdlqdcbfv.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fehbvm.com/Article/details/gyvjiracc.sHtML

[S54] C++：异常处理
来源：http://blog.zdbjq.cn/Article/details/gklblbtji.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/gavyunzyy.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fehbvm.com/Article/details/gsarqllfy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/gxbkqhigl.sHtML

[S56] C++：optional
来源：http://wap.zdbjq.cn/Article/details/gpevzyten.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fehbvm.com/Article/details/gtngqvwoz.sHtML

[S57] C++：编译期常量
来源：http://www.share.zdbjq.cn/Article/details/goicndcdo.sHtML

constexpr int N = 10;
来源：http://baike.zdbjq.cn/Article/details/gdiczsolg.sHtML

[S58] C++：命名空间
来源：http://read.share.zdbjq.cn/Article/details/ggdqhnstp.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.hesvh.cn/Article/details/gwhqmlyxe.sHtML

[S59] C++：静态断言
来源：http://mobile.hesvh.cn/Article/details/gqixvqgul.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.hesvh.cn/Article/details/gaokrxvle.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/glxxtvfiq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.hesvh.cn/Article/details/genwmdxoz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvvoiqliy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gomkmqbkg.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggcwvgpch.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gspnzhkco.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gnswoskjd.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/gqayviuum.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.hesvh.cn/Article/details/gummwvdxl.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fehbvm.com/Article/details/grlyxbsyf.sHtML

"值: $b"
来源：http://blog.fehbvm.com/Article/details/gxgiwuaus.sHtML

[T04] Kotlin：空安全
来源：http://baike.fehbvm.com/Article/details/gnicibhpm.sHtML

val n: String? = null;  n?.length
来源：http://m.share.zdbjq.cn/Article/details/gjnnkjniz.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/ggrmucdfl.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.zdbjq.cn/Article/details/gdolhogpx.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fehbvm.com/Article/details/gcnvvxwoe.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/ghkdkgixd.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.zdbjq.cn/Article/details/gfewphwpt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.hesvh.cn/Article/details/gcxcavmwk.sHtML

[T08] Kotlin：数据类
来源：http://blog.hesvh.cn/Article/details/gzasomcky.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gbhbtfyiq.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.zdbjq.cn/Article/details/gxkzbdogl.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/gzfxcmygt.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.hesvh.cn/Article/details/ghoczncxp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/gxpwgbaif.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fehbvm.com/Article/details/gsmzgkqww.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.hesvh.cn/Article/details/gakqffzto.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fehbvm.com/Article/details/gkkknuqrp.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gwwnnennp.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fehbvm.com/Article/details/gabpfxmcj.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fehbvm.com/Article/details/gznlqpmxc.sHtML

[T14] Kotlin：循环
来源：http://baike.fehbvm.com/Article/details/gryarolvs.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fehbvm.com/Article/details/gjeaqerrn.sHtML

[T15] Kotlin：接口
来源：http://read.share.zdbjq.cn/Article/details/gryjahdop.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.zdbjq.cn/Article/details/gdnxzhehs.sHtML

[T16] Swift：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gdadcaafe.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/gzlsllokg.sHtML

[T17] Swift：变量与常量
来源：http://read.share.hesvh.cn/Article/details/gcwbczktf.sHtML

var a = 1;  let b = 2
来源：http://wap.zdbjq.cn/Article/details/gtotqpxkr.sHtML

[T18] Swift：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gguinvkdn.sHtML

"值: \(b)"
来源：http://wap.hesvh.cn/Article/details/gyacqcdky.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gjyhkiwuo.sHtML

if let n = opt { print(n) }
来源：http://3g.hesvh.cn/Article/details/gajqgwhnm.sHtML

[T20] Swift：数组操作
来源：http://mobile.zdbjq.cn/Article/details/ggglcglrw.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://3g.zdbjq.cn/Article/details/gllxkozrv.sHtML

[T21] Swift：遍历
来源：http://mobile.hesvh.cn/Article/details/gxgbketlf.sHtML

for x in a { print(x) }
来源：http://wap.fehbvm.com/Article/details/gucnqbsqg.sHtML

[T22] Swift：字典
来源：http://blog.zdbjq.cn/Article/details/ghnfbsrnw.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/gbswmkvkg.sHtML

[T23] Swift：函数
来源：http://www.share.hesvh.cn/Article/details/gfejsvknb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.zdbjq.cn/Article/details/gwjbankml.sHtML

[T24] Swift：闭包
来源：http://www.share.zdbjq.cn/Article/details/gqrdhzehz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.hesvh.cn/Article/details/gsymolagm.sHtML

[T25] Swift：结构体
来源：http://www.m.share.hesvh.cn/Article/details/gxleckktp.sHtML

struct P { var x: Int }
来源：http://www.blog.hesvh.cn/Article/details/glrygijts.sHtML

[T26] Swift：类与重写
来源：http://3g.fehbvm.com/Article/details/gwgxbghao.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fehbvm.com/Article/details/gxrpdmuom.sHtML

[T27] Swift：错误处理
来源：http://blog.hesvh.cn/Article/details/gllrpscgj.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fehbvm.com/Article/details/gjgedbfyi.sHtML

[T28] Swift：枚举
来源：http://www.blog.hesvh.cn/Article/details/gckvvybib.sHtML

enum Color { case red, green }
来源：http://3g.fehbvm.com/Article/details/gqshhoamg.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fehbvm.com/Article/details/gzgswxvak.sHtML

guard let x = opt else { return }
来源：http://3g.hesvh.cn/Article/details/gliakyxgs.sHtML

[T30] Swift：协议
来源：http://mobile.fehbvm.com/Article/details/gurrqbpay.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.hesvh.cn/Article/details/gxoajbkzd.sHtML

[T31] Lua：Hello World
来源：http://blog.hesvh.cn/Article/details/gqnswenvo.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/gvnvaltzx.sHtML

[T32] Lua：局部变量
来源：http://wap.hesvh.cn/Article/details/gwsqrfyla.sHtML

local a = 1
来源：http://m.share.zdbjq.cn/Article/details/gagpldocj.sHtML


<!-- 参考信息 -->