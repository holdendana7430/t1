代发 wailian999

esac
来源：http://www.52xcode.cn/Article/details/gt2svgxkcfd.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2abyexfwt.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2rihcdozr.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ubwpuswo.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2dmqzgorp.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2dgctjsdv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2earfjfsa.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2woodtlir.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bgsiwlxz.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2qwlxfmgw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2krhzjnye.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2qqwpnirq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2trxtljvx.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2zpouxpfe.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2gedpdbxg.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2phabximz.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ygqmxsxl.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2dcrihavl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2mjdvqbvx.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2dmlbzjgw.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2gciacdxh.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2wunztmhc.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2inqecleg.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2eggwhbvo.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2ytpjkftz.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2bgwcfaxp.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2jiuxbxaa.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2ivlsankb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2odlmqfal.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2oaysgkol.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2joazyiat.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2entghndh.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2gwenaqnp.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2klowyods.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2wolcgxsw.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2okyggqng.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2pxbztmyb.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2agdgxgid.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2uvubuxdv.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2hhoifqnl.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jzvihdsp.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2ccycjtyf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2wegobfjj.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2jxocepne.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2apcvzidy.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2oezzlucw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2glgdewsa.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2xzlhgwsi.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2ngtkraqz.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2uzkzebhx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2rrbjyotn.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2gwjnovoi.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2hqwjllat.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2wkyjuhfh.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2ahypffew.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2krtbrupq.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ncuvppiw.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2jlzzldrx.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2zuwimujk.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2pwdvrobc.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2zjyxhvvu.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2hequfohf.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2xjlbqyzj.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2vgcmvwfw.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2uymsvjai.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2ltpihbbn.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2mkidistj.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2jetpkitw.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2qpiwobdv.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2tiumheyj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2kjrdbgoo.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2tehcscyv.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rfvnuyxe.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2bxitzffa.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2gntlwiic.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2ziywklam.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2mhtgvrrw.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2bitxaphf.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2jcboptll.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2vfrwjznl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2lhlganjy.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2bjskarjz.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2barsexcm.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2whhcmtwf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2pjkrqvik.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2eexvglwg.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2mmihnhyg.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2rmchnspm.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2qboukemq.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2biqslfky.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2pyqgmmuf.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2qzziphrc.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2tevxeatc.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2pnefpczp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2vdrgssqm.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2sbppcxpx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2zmnitlbd.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2pwxyaznp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2xujcyynz.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2jlzvrvxg.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2hzwzdcwb.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2siaftldh.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2bhhukwzm.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2cytwcnzp.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2hqwtwpgp.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2txyebitj.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2jdtoiokj.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2gumusmwn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2fmnloazt.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ukupctfz.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2kmodghlb.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2nfmykwuu.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2ajcdcucv.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2cvvcwniv.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2hdpzedxb.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2xjrrakbd.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2issqzetg.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2ulrwbaon.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2lqdsblpc.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2slgdqkmq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2eepylwjv.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2qdegkekv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2edhgtxki.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2nflfmkzk.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2dxmvkqcp.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2vtltmkxo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ierivpmm.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2hvmokfhc.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2pjmmnmzi.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2lpaistma.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2icxwwunn.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2gtwnobag.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2umvyljlt.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2mdihntla.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2lacddfnv.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2dfgqjxrd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2fvdrjyya.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2qbwpreyv.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2shxzfriz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jkpsjtpn.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2roufhlmr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2civnufpr.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rhckqdfr.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2fojvdlbz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2vekhygwi.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2vfkcpbhl.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2qqaoelyt.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2rfyioevp.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2cjmilwkq.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2ogommofm.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2pikqloly.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ydxreniw.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2kvnpbmxr.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2deonyrcz.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2xrtfsedr.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2ugghaxko.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2aomruzzq.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2xqwxuzyx.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2haoowhhr.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2xtccyxiy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2gxpsqapr.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2crcoqyag.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2pjtpnuvh.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2zixmogfh.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2ycxltpsd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2epopnkqk.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ppdrhwpg.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2mzvrcshg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ivcxcsbp.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2xoqltacv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2izdglpru.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2wycmxfzy.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2wemqtnvt.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2alvtgblh.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2xvspcnbe.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2lwaphfbf.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rybgmgkx.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2nooqvqle.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2jqprtcco.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2pwjjjazb.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2alklsoqn.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2prsfixjk.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2jwbburdh.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2jjsijqol.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2urvhgttu.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2salytpgd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2uvxrdxew.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2afjoejjo.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2tnhubihw.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2lpqfaxwv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2hjqwwjky.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2oumzlzwd.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2reskwvwi.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2hunherog.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2ecsgaiff.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2kohnbsbm.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2jjzolndc.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2ujknwvpu.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2glrwahsg.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2byzmtgmh.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2raxbethr.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2hmhjkrdj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2zmrttblk.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2figyjeqc.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ijlhkrmt.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2emurprwg.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2nundfgwc.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vhyfxzou.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2hbrajfbm.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2chqzvtjq.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2qbjdcscy.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2yhocnfnf.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2leviiwxr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2xednunnx.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2hqwipqkl.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2uybmdsje.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2cedmotul.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bcvrzqsn.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2hanmrpvs.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tvhxekpv.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2fhmfufif.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2txvaupvw.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2zhfmcpyu.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2lexabaag.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2fnmvammf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2nijknlwl.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2khokbpyl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bvxnqxjl.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2puavhwji.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2huxynpry.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2slukfgbn.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2dcjjzani.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2wkqggyax.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2kelimyxw.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2ycvwkynh.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2rcjffxvn.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2ofweidrh.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2thyqlsvo.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2jupadiwc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2ewzeakzl.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zaxyiblg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2nsowgxaq.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2dpezrnwq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2lkxpcvmv.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2gavhljhs.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2wsxcfpbj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2aemydgxc.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2regjxzig.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2bzokuqdl.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2jxuefzvk.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2dwniwprx.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2hhiwdghi.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2gsdwspdb.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2nbtsncpc.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2ioqumnpy.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2nbtzitav.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2yiklqqdn.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2tzmsfevk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hzirvsxt.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2oazxsmca.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2amdfizcp.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2mhccxhvq.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2jforwkbd.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2lxnvghqy.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2uhnmewav.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2dutynpqk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2ujuucymi.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2emgpbmsk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2qnkngicb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kplevcnk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2iimpsumj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zhrlzjjj.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jdfnbvpa.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2tqubxbbw.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2bnfseaqc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2olewhxae.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2aogkjido.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ryxawzhj.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2zmyejako.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2giwjbfvq.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2qfmtreky.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2ngobkflc.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2sijzsmgp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2naasdesf.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2sbzrycxb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2tafnvkky.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2rkipvwvb.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2gimqrher.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2zhynqgdh.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2igfrygyy.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2clhyluko.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2cxebujls.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2cxaxidep.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2jxhvpzxv.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2ycicogrf.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2epysltes.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2kxafplhc.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kzzucttc.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2mmzxxruh.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ichjomuk.html


<!-- 参考信息 -->