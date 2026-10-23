代发 wailian999

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3aidvamku.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3cjmqvoeu.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3xianzdyy.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3lhkrtmar.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3vinzungz.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3lnmwfuhh.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3uuuawkrc.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3dofkninu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3asfkvlvj.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3ngexwgbt.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3jxbrdqzh.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3pvkktdvm.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3mqwllgjq.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3xakzhvam.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3pxqfsxeo.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3vjmhnmmd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3jpcrcdck.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3iotibdwr.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3uupypyxw.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3youjaxzo.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3nipyaxnw.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3avwuzxip.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3qeorwmyl.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3kqjaksdp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3nmyfrsjc.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3gycvruhl.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3eavuxhan.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3zdwmarma.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3hfnnsqho.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3kkuzdgiw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3fynofwxo.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3fatquyhs.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3mkpomftc.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3iejpovkc.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3rkkguefc.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3wxdwnxaf.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3yscaeqky.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3wfefjzzd.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3irymnoga.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3zdmxfifx.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3fbiufrid.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3kwidmjqp.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ujyoqjof.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3ulmsftko.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3tsaqkbmy.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3orhiosrm.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3mtjdbnpr.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3ujfhfvem.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3kmquejxa.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3ajoxcgdc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3oxpruuov.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3lglvfkfx.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3edmooshw.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3wnyqplqc.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3vgylkqct.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3nagjrzlw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3dxwhovhp.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3cyninkrs.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3iecijzyq.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3xkvbdcqy.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3ndndkvrq.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3hpdxfbeh.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bsdbridd.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3kkqgudyn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3jdxjsadj.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3wvtmxhkw.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jzduhptf.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3gchyjepi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3ltozgxjm.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3rwnfjvhg.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3jhftwkrl.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3emikjwhd.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3pxjzyjxa.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3hrkyyugl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3fncqrswy.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3acdjsuih.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3qsunekzh.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3azhoygvg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3amuiipfb.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3gqefrycl.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3sfsuciwo.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3oohmlsyl.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3bgasirlv.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3nualjown.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3kchipptm.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3emdydxct.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3qlariydo.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3xhazgxtp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3dofqtkwc.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3fzdztqdv.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3ltvkpguw.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3ehrepmcd.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3wkohgcaa.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3tejutpje.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kdilnowg.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3pqhrdapl.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3vgnnvhzz.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3usbcisbc.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3uvmuluah.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3bcqexebt.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3ctbtquku.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3gbchykzj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3vegwdqdv.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3jityvgpf.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3bahzncpt.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3nnkuzxsa.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3cdagjxsu.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3yabcnhpd.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3oinijoti.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3muqmahjw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3zdxthjdk.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3phulkxar.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3jnvgbhul.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3wwxrgree.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3dcqniogq.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3qmmmwpmk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3pjngohmn.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3clnhsiqv.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3vsjcennk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tacvozei.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3hbyfsrxp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3awrptyuk.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qmwtqvbf.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3gsghcwhk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3agtswtnv.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3wdyrhnqw.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3nmkqkcqo.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3neteuefj.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3gfotnhea.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3dkvjtlrk.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3rkyqecjj.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3iudoiypt.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qglhstvk.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3kojljwix.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3acsiqrqi.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3qbldxnbf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3vmxbetbc.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3fbucgyyp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3nexnxrag.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3rzleodtf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3irahdmes.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3zkdzhxjd.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3gdguwqyk.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3rdozrasz.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3jttlpqgc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3mdcmjtqp.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3xjlurcrf.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3nlxlspwx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ftmqcahq.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3mivgksdm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3dgfoerhj.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3rayewasj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3wocqccxd.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3sohnbcue.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3hlwulgsn.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3pomkbhti.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mczkosbh.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ofdcjdah.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3aijticcz.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3cswemxwx.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3ljabtohg.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3dlivfevz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3rwzblwno.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3xwuhvvhu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3hvfcqegr.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3rzgzddsd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3zelhibwf.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3nvnnetfl.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3gimiujzx.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3cgllqzfq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3fgvmrjfl.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3arlqspwx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3jjkaivgz.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3lejuquug.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3qhwqymvb.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3ltrkhytc.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3alprzxmo.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3musqasju.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ehtnoplo.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3wcphlvql.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3twhbhckb.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3ewdczadu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3bbqjeyik.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3pkzaiktk.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3kxczpgon.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ocioyimc.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3mnrifkmk.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ylsgqfjl.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3vhqttghz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3svaetcxz.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3drvyevia.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3wthjnnvn.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3hikzejaj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ukhabhxh.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3uxmngegm.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3lhrpfezk.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3tgbdyelw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3jotngbmb.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3tpnwymly.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ivxetzjy.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3pmvpyuqd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3qritjlfi.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3pfbbudvl.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3nzkfzafz.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3atjyfuvp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3nkpxpjzg.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3oniplnfb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3ixrevpty.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3occjpenv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3kpldrtrc.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3fxxcdpzo.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3pownpccx.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3lepznjlj.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3rfzjcint.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3mbygsqdt.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ikrvmxgd.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3egiousvm.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3lokhaxbp.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3hyibmijl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3czwxbmee.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3otomcrfs.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3xizuxwgs.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rzieazvu.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3gbdgnxqm.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3sibbwyof.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3ojqzutav.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3swsctbej.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3dbhwskpw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xwphtbiz.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3eoihpqqf.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3sbttkudt.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3vnsccimv.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3nlppzjqf.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3cyimjqwu.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3wwmonaat.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3akarperh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3bglacvox.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3tyzhgmok.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3zipdvsha.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3lsolrura.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3rgngmfri.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3lfdfyuev.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3ehumibik.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3bekvzxkd.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3jlbqkgxq.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3lmbllsiw.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3yvzdfegw.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3bqdukdin.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3pjdnxlbw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fxvhbnce.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3bamzghsc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fmvjvrgj.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jparciei.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3atxaltji.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3tpyaawzp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3nxukpjie.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3ibpasddp.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3vzdwjpzr.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3sgxarwiw.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3jxhmpzzl.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3fvjexvqn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3dhuejboa.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ttgwxmxu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3byjdqjch.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jfxcsmrt.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3bqubanlt.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3yqyatsjl.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3kugqiemj.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3fmrbkjsn.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3wujnswbu.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3hezbnwkj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3upkkmyav.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3ohfczoou.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3cnufcgxb.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3zszoaudk.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3enhpzysj.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3fpbixpon.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nehgnvcj.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3ssznwzec.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3hfhjvuna.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3attgamnh.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3ytmxuhqq.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3oxusxckg.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ezmbuoiq.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3xlmaodaz.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xophkigs.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3nexnfajg.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3pegwnxax.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3ejwhjgbk.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3jtburuzk.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3chhjachp.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3mstldyni.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rwjjcods.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3xblwzwrz.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3rkasywgw.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3ztxotmla.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3otiymgrg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3tfouzyoj.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3oqxabqgc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3dzqsvtsb.html


<!-- 参考信息 -->