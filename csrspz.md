代发 wailian999

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3zmjlsufx.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ispwbacs.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3cvdnveti.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3xjazobuh.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3mctmxkgq.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3dbmhrapt.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3ddlmfkup.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3rcamvofu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3lhonpaxt.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3awkjsauu.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3yreakusk.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3yxcpwcov.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3syinavmr.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3bohcjdgl.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3nxozzqnj.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ikegxsar.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3gahwswji.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3ipgnbgww.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3mzqqdchb.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3wpcpocff.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vcrcecpw.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3vysdzasm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3gapsdwxo.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3hejsrtwy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3afpxmsno.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3vaptsjuj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3mskdrjqe.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3szbljlvs.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3jvxhoqmn.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3hwqwjvja.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3aueqxsyl.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3jdzbyshv.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3vttffeye.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3hhzgktjk.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3gjyracgt.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3avreoijq.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3vfyulohs.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3eojuiwfx.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3ppicvmwu.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3xqvkegfw.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3yafllhjd.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3papkyypk.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3qwlbpjcz.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3kwiurhaj.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3ckypcffv.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3cmkbtfyg.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3uyrnqhdt.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3eotobmwt.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3dkivvumg.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3khjpdego.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3peukuygn.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3sopqttau.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bfilisay.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3acoiumbg.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3rjwkzwkz.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3grwjthfu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3kiyeeklt.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3qgupfndy.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3indcbvie.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3ogjnjjvf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3ikmpzigc.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3ttpktcjy.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3eryahekr.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3sphemoml.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3ykmceuon.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3igfwwzgj.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3rmnmjfgw.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3hfekepes.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3twdogupf.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3azwyeufj.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3esboltcg.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3zignyegl.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3dtmykhxn.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3pgbsrrdp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3exkciltm.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3vsahdbmj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3kjoazfxh.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3bobshjyn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3fcmwjrrh.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3hhcnhwrp.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3ehjowwdz.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3npozvkng.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3xakmtiwm.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3wgnxmbwf.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3kqiqosgm.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3qrlmmacj.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3reojfdbn.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3mlnpuwyc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3vfwaryqb.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3xvhvkwut.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3nndzvtpo.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3nlzpqirm.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3kxzaohmq.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3iinuanfn.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3cgbeezmr.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3mxyelokt.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3yokljbqt.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3lipbjkuz.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3zmqzgwsa.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3pgqqixzd.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3ogmibgpb.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3bfgzypor.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3upxkwirj.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3ypqgqdex.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3nwgetdny.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3adjdqpdb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ievcsjik.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ycqcyncx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3gqudhtzd.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3bsilntxq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3jxiqnzqu.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3ifdftgjp.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3urdhccmc.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3qensurlc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3jiqtdfol.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3hcprzuuy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3xlfobkgg.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3vqwnmzkt.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3gkoskibf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jjjoyrqs.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3jfuyxglt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ojmiyxlh.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lvkfdtjk.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3cohcdmon.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3wbdhxdzo.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3inecllhg.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3ijbhdhpa.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3khytojrg.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3erhqxuvr.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3oxvervas.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3casravzn.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3mvcjuqgw.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mwmclymg.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3xsxoshdd.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3zfwswquj.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3fhdserhy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3gbgexkpi.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3ghatdbfj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3ffgrzxze.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3utwupshp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3hujizkgr.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3eweespzp.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3gdebyqlt.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3feccprvr.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3tqvqvheo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3mdcuikot.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3qwdmktif.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3mpsoyaro.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3vhamyucq.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3lsosaqzx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3splinebi.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3hqkoegzy.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3lrqoyjac.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3tqdsotth.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3kngmmrrt.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3nqcfybwb.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3eqjtjxtw.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3gabwxdzl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3stcsipgx.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3iofsdthn.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3lcnebaon.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3rvponxwa.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3zwbfiqqq.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3ityvigmq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3oqpzjpzt.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3jvnjraoy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3kutzyucz.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3iedkwanw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3rkmkwfiv.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3tjliteje.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3pfsgmihg.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3ltdcjzyv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3labqkirm.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3cikbweug.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3ymupzigt.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3qoozsziz.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3bxiyxtua.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3povvmmuc.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3oqiibqbp.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3indyprvc.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3qcnnqgap.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3tgfffoko.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3icwxddvq.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3fztkfcou.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ygxwzciw.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ueaaypkr.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3jmktmkif.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3hgchvvzx.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3hcmbayxo.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3perkeunc.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lwvjtxrm.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3adrsfhor.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3fgwtpooi.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3veyzlhob.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3btekehmx.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3wyoagasv.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3ggbrhwpv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3cfshcsrh.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3imdfhvcr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gvtdzzul.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3hwnczxgi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mmtywung.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3bcivqvxl.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ncsigndo.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3kvsofmqc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3ohksyvsb.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3sovnjczk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3zmmzkunh.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3jngkpiww.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3eaqbpqwc.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3arpkjjhk.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3ikkepvop.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3hfhkzxey.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3xhjxhpoq.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3xnetmbdy.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3sqrsgarq.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3fuzaatpo.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3rbjehski.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3vagjhqpm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3cbyxmxps.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3igomghnj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3lmoddqaw.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3eawubxan.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3vnwhjmmd.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3jhfefjay.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3zkeuzycf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3tzjnayxk.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3ldrqqhup.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dljnjpzp.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3bnkgeynv.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3zphumanw.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3yxegqhgu.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3vjchhawz.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3tnjklmmx.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3bebhyxhx.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3cufxihar.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3tbxgzjfi.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3mnmxcgis.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3taatwrvu.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3xbuttval.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3tssgxntu.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3okmpiyjl.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3cdmwgnaf.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3ganxdaud.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3dtcaphaw.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3dfpshnes.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3nwcvjkys.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3doqjqdyp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3dkoyupnq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3htkdxkpp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3drncifxf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mcphhbsp.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3exnqskkr.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ekuagrss.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ynhlwmcz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3lbjcfvne.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3rbntqywg.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3jsfwlino.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3kgjjqukq.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3dznssmix.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3xpuspdrp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3lggfeuyi.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3nmdrhcqq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ziaspqoh.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qafgrljx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3ysxtbqdx.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3fdquuftw.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3gpzjwaoc.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3ubkjualk.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3jilismgw.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ldbfugfh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3vlveuctf.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3lbznztwy.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3reucuwrm.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3mpfdfrix.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qbqdgrtc.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3krrgyjyf.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3dcchtvrz.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3kjuroitc.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ycmqerqa.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3zcpfeyzc.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3xljgcphi.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pjczysnz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3rvldcmtz.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3rhfwlpwb.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3xagzddjn.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3uoippsmd.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3eovhowlm.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3ksyqxjax.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3rzjiongj.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3aqoxlirn.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3nlraruki.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3oeqqwecy.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3tzmobypo.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3ixjjxxzn.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3icaatoqm.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3awekxfri.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3qwxhcbjz.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3ympphczp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3beyaelod.html


<!-- 参考信息 -->