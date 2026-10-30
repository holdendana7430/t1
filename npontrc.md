代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkhemzsn.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gedajcyhz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/gwicfvnmp.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gpqiceogr.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnyafzcmo.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gfqislslr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzjotvwa.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gsecpzkpk.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gppeyuwkn.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gygwevgnd.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrfhziis.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/gnoifuwta.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjjfzyen.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gzpaykcda.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gilbahcpu.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmjkyzhq.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gshbgmirp.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gidlpokte.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gkoojdlja.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gjurfntqs.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gcdrkxapp.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gdwjbqyup.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlitmhdr.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/gqhlktgux.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gszvnzryz.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpbqqtrk.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gporctwbf.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gbxkurfqt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjkavxyt.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gjiwnlces.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvhpvpox.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gqyunxyll.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/gwvpebfqh.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/gorwebmbd.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gqbemypql.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/guikfxsxt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/gmctsudbd.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gporosepw.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gudsuyoqk.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/gpkbdugsw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gijyvrmeh.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gkahqahqx.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsaoluvnc.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjhkukgk.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgquogls.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gstwysbyz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfuixrdq.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gnqrbuzrt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/gojirfdou.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfpkpdrw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxtvgrot.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gjucfyeuc.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gmsjwxfyk.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gaiccanuc.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/ghvivfokl.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/guwzcmojt.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/gbcctfhyw.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/ggsirrung.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/gghphifmk.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/gxkcpbmxy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaylezcpm.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gsynkwsvo.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzncfpxx.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gyrydstzz.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/ggisjgsjw.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gxmhwkfxx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gtdqiojwm.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmzuivwv.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/gqhzajthe.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/glzliodws.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fanxiaobao.xyz/Article/details/gseirenws.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjthfddm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/gqklpmtqe.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/gouaislun.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gkospzfdh.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/geprmpozt.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/guaojvkeg.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/gcngzcmrt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gywqvbcpd.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsjpkjiz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggznnszix.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ggsrqprnj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwbllcub.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhpcwehk.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/gipsvcjrz.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gkzutkmkp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/grdzzkwsp.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtbfdbhn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gcoighbyw.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gakbjzrst.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/guetfebki.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjbacnbf.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/geamwpvyu.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gvmpgpajy.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/guhiphgqy.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhegoimk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwiqrgtvs.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gwetayfre.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gieyvseop.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/guiiumjkg.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girbfixus.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gzodqekjs.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/golsajndy.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfwztson.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gckxgoqlu.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gwovdwhtn.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/ghvgbyfov.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gzyhvtlwo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gocfrengt.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gyveecskr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimhrjgcg.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/giitbfmrz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gaxamszag.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/giikcddtq.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gchpicwdv.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkcajixc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/ggcfhvxmr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gosueincj.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkikpyqf.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqhikstl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gpyjdcwki.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gschoxbrv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gyrwgkgib.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvkfhvix.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gpupwsopl.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkhsmztt.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgikzuma.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/grcxwebzl.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gvhladeul.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gqbaxeuvl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/glfxzbhum.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdduxrbrj.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjywvsmvo.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gzmvdjxoc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxugkfbp.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/gxijcikzh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwgbrhwni.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxyuvdga.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlsygamk.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/ghartwvzi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gebgcnquy.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gbvmuhysg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnodxaka.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/goaqyrsgt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gagxprslg.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/glqhuiaja.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gvbbnvbix.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpideljoj.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunifjymk.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gqmvjteqe.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gliwnxbwm.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/gepvizhdw.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjymuazf.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrqjoasj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqexblgrp.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/grcqtangj.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdalpylp.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gvodfrefo.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhfsuygv.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrscgnbb.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywkspind.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkfnszky.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/girrxqpnn.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gcaddiodq.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gvbkhmpxy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gfctossqn.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/gaqsjatkg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gabkkkciw.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gqlqhzrzg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gyxmfflod.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gacgadygq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkelqxsp.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/glhvjevsw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelnjoajc.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gomdtuwiq.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbmifibu.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/gcrdhzsio.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjebslgjr.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gnqnptmqv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvranjox.sHtML

[S41] C++：类与构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/gxwcgvprm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmgacgaz.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxgjlooa.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/gzcintyca.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjlwmcwj.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gawrnptvk.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftempnln.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gfjymzcdd.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbzgilys.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhybukvr.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqbfqyhv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gtjckryep.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gintaffgf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujanoraa.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gddfmudwm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/gkbitixnp.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnrkeqxu.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gjnumpmro.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gwsxkwius.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/gjssiygts.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gjgcbztct.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gaiuloodk.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gllmwmund.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/gagqndwoz.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvqsckftn.sHtML

[S53] C++：移动语义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchndcaqb.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvhwbzcy.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwnoywvf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gouyhvohw.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaujzkhlm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/grtmxhope.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gumspoclb.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqljdflbn.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkpkmyuo.sHtML

constexpr int N = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/girdkqwed.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswoiysef.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gfkmfyimz.sHtML

[S59] C++：静态断言
来源：http://blog.fanxiaobao.xyz/Article/details/gwahmzoqn.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjgkpzoe.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/gqnyraglo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gbxkczuyh.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gvrgmajfa.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwzlguzy.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqjacmho.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gfihkwgam.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gailtjrgx.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/giopewzdm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/gondaqxvv.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/guglbizgs.sHtML

"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gfagmplnu.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/giatvekgt.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fanxiaobao.xyz/Article/details/grohndxgt.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gfkzkvncr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahnmfzep.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbehtdbh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/ghrtmtzwz.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/giysmwile.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fanxiaobao.xyz/Article/details/ggtsbuyjb.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjjnuasl.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gowtozunn.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghugpvykv.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjmbtbmu.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhagjqca.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatjxkvot.sHtML

[T11] Kotlin：协程
来源：http://3g.fanxiaobao.xyz/Article/details/gzxsznkbk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fanxiaobao.xyz/Article/details/glnzhzjqw.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fanxiaobao.xyz/Article/details/gmpxxjcir.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gwmbmpyht.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/grgvgxrax.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/grneenqmb.sHtML

[T14] Kotlin：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gggvenvmu.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghisfwdue.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfaksyqxe.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gzbblswuv.sHtML

[T16] Swift：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gbyzkciqt.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/glizrotxp.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fanxiaobao.xyz/Article/details/grtuxjlbs.sHtML

var a = 1;  let b = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfywoptdz.sHtML

[T18] Swift：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gebdmxksk.sHtML

"值: \(b)"
来源：http://baike.fanxiaobao.xyz/Article/details/gsovkgcbp.sHtML

[T19] Swift：可选绑定
来源：http://baike.fanxiaobao.xyz/Article/details/gjlwkryom.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcavtpvqf.sHtML

[T20] Swift：数组操作
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpgukmlt.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkyjcbcz.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbwgvape.sHtML

for x in a { print(x) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjaxijsx.sHtML

[T22] Swift：字典
来源：http://baike.fanxiaobao.xyz/Article/details/gbwnbvmqx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gpgcneabu.sHtML

[T23] Swift：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpqjkeeg.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslkuabzh.sHtML

[T24] Swift：闭包
来源：http://wap.fanxiaobao.xyz/Article/details/gzlvsekvd.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gfvnlmdly.sHtML

[T25] Swift：结构体
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzzwoctm.sHtML

struct P { var x: Int }
来源：http://baike.fanxiaobao.xyz/Article/details/grepawfan.sHtML

[T26] Swift：类与重写
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvjbfoqa.sHtML

class A: Base { override func f() {} }
来源：http://wap.fanxiaobao.xyz/Article/details/gcxyohzwt.sHtML

[T27] Swift：错误处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gicvpaorq.sHtML

do { try f() } catch { print(error) }
来源：http://3g.fanxiaobao.xyz/Article/details/gdaieunjz.sHtML

[T28] Swift：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gioaqlcrm.sHtML

enum Color { case red, green }
来源：http://baike.fanxiaobao.xyz/Article/details/gpnczvyqx.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fanxiaobao.xyz/Article/details/gtnjhhmqy.sHtML

guard let x = opt else { return }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhtpvgxk.sHtML

[T30] Swift：协议
来源：http://m.share.fanxiaobao.xyz/Article/details/gndfrdvfd.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnamvnsh.sHtML

[T31] Lua：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gogxvivmd.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdzqamyt.sHtML

[T32] Lua：局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gazdfjwae.sHtML

local a = 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlfomkwy.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtniltbfa.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fanxiaobao.xyz/Article/details/gjvoocnre.sHtML

[T34] Lua：遍历表
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhvbgvvg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fanxiaobao.xyz/Article/details/ggruvtgll.sHtML

[T35] Lua：字典表
来源：http://baike.fanxiaobao.xyz/Article/details/gudvtehql.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gugqlakvl.sHtML

[T36] Lua：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gziqncpdy.sHtML

function add(a, b) return a + b end
来源：http://wap.fanxiaobao.xyz/Article/details/gqisqmkwc.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubyhowxl.sHtML

"a" .. "b"
来源：http://wap.fanxiaobao.xyz/Article/details/gmptcfelr.sHtML

[T38] Lua：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gyqaanwjg.sHtML

if x > 0 then print("正") end
来源：http://wap.fanxiaobao.xyz/Article/details/gmbgcobgv.sHtML


<!-- 参考信息 -->