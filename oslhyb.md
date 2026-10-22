代发 wailian999

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2yrcvlkor.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2fuodtvzs.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2qleieqto.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2awvukqyq.html

esac
来源：http://www.52xcode.cn/Article/details/gt2wvipzrtk.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2pyfboyqy.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2ckfmwogv.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2swjfqffc.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2akbvxtor.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2ydyzxshl.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2tindcftv.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2sylmqvlw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2ckdpyksi.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2lfaqdpxy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2fbyhnkpn.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2tohlihiv.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2rrpjzloi.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2rfjzmkos.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2lrlhikta.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2mtnwuzny.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2tlqvhmrq.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2akbpclce.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2ngvaxcot.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2mgorbnop.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2khpwwudv.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2cvcwvuwx.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2krqaayxh.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2owxdjrpz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2pyqlppcc.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2rwvydpgm.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2krhqdixf.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2vlvqkuyl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2spokrvls.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2gjryzdrk.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2bloylzfc.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2ggwjqsrt.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2didllsse.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2imtsqqog.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2lmeiuhto.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2zlrjxlbj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2vacknkss.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2sgkdxfew.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2sykoqvic.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2qmabltsl.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2diblrexg.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2wuubycmf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ghshuehc.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2xhfemvrd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2ssnbhmqv.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2uicmpppq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2albmpsxa.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2fcoygstj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2zehumncc.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2uhzupfzw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2plnutdhu.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2nluwujqg.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2abgdtxwj.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2sydhxmpu.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2hgtmoanv.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2twaqfznc.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ojgaecor.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2awapgnwg.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2xhitsmer.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2wazgdeej.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2hutfwxcu.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2dlmtmnrz.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2ydhlvysy.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2jgraisgx.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2bsukynmb.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2dtxvgzxh.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2fmfufdmo.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2unzfqact.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2avseikoh.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2yeirhede.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2ugubprbs.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2fzvgfvac.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2xjvtmiyp.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2erdqdgei.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2qhxalqin.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2valvbpzj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2xgeeopac.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2qulmsaqg.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2znpkerxz.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2iguhwfiy.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2gndqvpmq.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2ujdmdweq.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2dijcqnan.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2qpoweaxl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2yvoamgvv.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2iezbondd.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2alwodcpo.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2frgyejpa.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2fivjpabg.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2ouzeysfl.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2sqqlzeus.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2gmfvnltp.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2zvpgfgah.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2uozfmple.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2gjgsmmsy.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2wxgmepmg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2wwbnqtxw.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ieqxjokn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2pskwvixu.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2vtxrhvsp.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2wzfgcvxh.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2nrhkaejc.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2clgpsyxx.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2jmwbdzyp.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2bvmhhftt.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2rirxjimh.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2ftxfwzfb.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2itmtzndx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2lsfncfxr.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2yutbkvhk.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2eizkubhq.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2lmmsfzgt.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2tthlngbi.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2wlzbneic.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2csbcuzcm.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2dcpikubr.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2nmufbgzl.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2hbysxtri.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2wtcatuvr.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2aftudgoz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2bsyxungj.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2kofhagzh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2taztaflz.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2dkicnbwt.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2pxdfjnze.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2ykdrjopu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cfqenqmo.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2hsewmzor.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2mpmlinbd.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2jewpexor.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2wcvmlwbj.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2qkvqxqow.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2yqxtsnis.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2iikgqcob.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2xyskpjdz.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2zynpxhlk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2dvfoepjs.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2lxfppkim.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2meanualq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kyymrhgm.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2qwwbcngy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tljesrcc.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ftvtjuch.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2lxeigyde.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2yircicfh.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2dzgrveww.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2fuqarosr.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2fbirkyvk.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2huiimdte.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2mvtcbmzw.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2juftnjri.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2wvihhfcy.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2gfwsqvvi.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2qziukxca.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2nykwjqsa.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2cxvmxriw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2pzvclkji.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2rtgbllof.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2vsgnosin.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2bfzztsny.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2zfmtywfh.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2fdnbiqbd.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2fmpbmlke.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2qvrmstqy.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2uyyrthdo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2pslnvxti.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2nkbuecmw.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2ksejstmb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2iwumltcq.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2lporpqhm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2ccgeoryd.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2epljxuxm.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2bltxbxru.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2rctmqkss.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2jzmeddnw.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2viqdoobl.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2oseauhwu.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2uqtfemnj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2pngglqdv.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2srcwnsrq.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2hycibkqq.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2tbhocahw.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2apzrwucx.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2dyhbmxwl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2vxgkptgm.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2lptmbatm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2bmazwujn.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2omgujalq.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2jrdbxmst.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2vuayiuia.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2yjiwdteq.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2efzyjhgx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2vdlrqazr.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2kdleijfe.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2bysuqtjt.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2xklxnpuu.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2pswnttmj.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2dcdhnbdw.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2evfhrjhd.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2hfwvuhph.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2bgitplkv.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2ufunhdwq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2xhwmhnwp.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2zjssmafl.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2tnywprye.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2xpcpcubj.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2gcvugcsu.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gocmacfw.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2ciyhsduq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ppwdbtaw.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2ctqrhsti.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2meryleht.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2vsxaxzke.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tybcvdqc.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2vlfzqcyk.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2bgrzlrjx.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2vvgtgvmw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lrocbjmg.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2hzbzycvr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2exmlacmf.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2ooomfktz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2suathhxw.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2uczpnngn.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2zjngrree.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2ccnnngrl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2ihkmqbuj.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2souhtyoz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zvqyxgph.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2rbqkuebr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2xrzflyxi.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2syvmjteg.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2tsltgrxo.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2xrhwgofd.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2mwuagccg.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2fsveumfr.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2kxlagsxi.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2kznhydag.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2qanlpsgb.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2nkkgdzrb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2ewwknzah.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nvtjutal.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2xrymyage.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wgybupfw.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2uyqfoslx.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ussjmndu.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ifzbpgxw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2vpccnhop.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2zfcbnujp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qezrteea.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2xwzquplg.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2gnfajkfr.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2crjjzxxr.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2kglofcfp.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2jfprsfed.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2clebceqt.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2ewpfzjue.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2xzadeutz.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2cmkyaath.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2xybklxvk.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2aoasabqk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2yqreevxl.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2whkwkkwq.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2booaafvb.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2isfylkra.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2vwsyiyjs.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2otzmnptv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2qmiwtjec.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2xgmtbhcd.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2bpmzlehf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pobcopml.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2mvlymecz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yxmjqyja.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2azbgujgg.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2mpbjdhkw.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2geekaysl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2oqemxbhr.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2saalozkx.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2xqnjhvyw.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2pawleoca.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2ewhgajvx.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qwctasiq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2xyyqadke.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2sxnxgsnj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vokuvaxs.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2dafgdvdv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2rnobguve.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ixznnjoo.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2inxlppaw.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2famzfdoh.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2msrdvcfa.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2sgtfxfia.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2fybfwzjc.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2iuxhxfwu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2pwdfbazz.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2rwcflito.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tpfbvqba.html


<!-- 参考信息 -->