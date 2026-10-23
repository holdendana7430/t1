代发 wailian999

esac
来源：http://www.52xcode.cn/Article/details/gt3lqtqgitu.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3ibhbnlzt.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nyjcajvj.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3kjssisht.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qzqzqcza.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3oqisuviw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3tnixgogd.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3drswmzxt.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3srnyesph.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3xndgusbe.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3lfneuutr.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3iyapfyeb.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3pwdiegtn.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3kfoogbcq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3mxbjyrje.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3zzzzxsqc.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3dzjafokk.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3dafgblud.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3ygkyfygq.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ckupptab.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3kdizwxpz.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3vgqnaznn.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3dsfynkdx.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3hnglzooy.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3pgvcbhlk.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3rqoceejm.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3xequqdij.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3vqjjoxgw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3izmkwwvs.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3gyflcxxa.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3nzknffwv.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3fgqtwans.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3visnruoj.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3zqzexgxx.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3wmmgdxaw.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3vgmlzbwb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3spunirux.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3gnelcgls.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3kxylyjxa.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3zhtbnenr.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ppodevnd.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3qwycwpvm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3znpenhjb.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3qvirltaw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3mqjgaqer.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3ywvzqfju.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ypkumdyj.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ttsadsvu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3kkrrgfev.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3vtdrzwmp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3mrwxwapi.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3jugbvihz.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3oofgbaff.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3rswdjvfg.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3wduirkoa.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3frhktiad.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3bhmnyooe.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3klsxsruk.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3gxjndaqg.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3tctcqdzb.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3tyiqiaqv.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3nnriphox.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3jnveyrxy.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3crmoxfev.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3pzzzjrhh.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3wqeensbi.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3cosicrii.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3klvcmplj.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3fuafhufq.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3jedtkctq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3ualginun.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3vdlusppe.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ytuhddjp.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3hhobjgkr.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3uxvdrbqp.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3wuqzldug.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3jyzrzahz.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3ufgjkxuv.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3altaynnq.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3pqppfzqc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3csthnrom.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3eajhhdvx.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yysbysam.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3fkvthhxy.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3bywhmxar.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ufvfcdno.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3oyenlhjq.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3neqzalye.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3sbshftja.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3yfcihbny.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3jthxpnnt.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3wslfvbkg.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3wfnkwczk.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3nojtpnbi.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3oqyhbabq.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3itlcioml.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3rsmrrcyz.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3cwylrxrs.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3njyqejpl.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3ydovvqrp.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3oyjgahfu.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3gbpydrmp.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3mfmptwuo.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3yjbnzpzr.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3zdwfkypk.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3zgjpnfky.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3cdsxmdcf.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3clryyqlr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3afbgkhcl.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3gxvxpukl.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3bunnbcnj.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3nfjfwbjg.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3djxcghlg.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3vozeturr.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vrxoaneg.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3menrsmfs.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3ldllaasi.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3zrubjeor.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3olrcvbtu.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ycarbkis.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3plxhsrja.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3nnncnfib.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3etrumiet.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3tcdtctmi.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3xjepbnsi.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3uezmvach.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3ztkaeyyz.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3plczhbkv.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3jaxnlxwe.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3luxiolcl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3nsrnzyhc.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3ttjqitjy.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3wewmaytd.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3urxpzwvp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3wczjjqex.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3qjlxcqzk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3tlfxtycf.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3fzzuupxv.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3rodcifeq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jdjmfgef.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3joipqrkg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dtdousld.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wzsummpj.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3rqpypwdh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3igioistw.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3epymofuu.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3gztffsdw.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3yjhbcinx.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3dqklilnp.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3sezwovpt.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3rgtrarti.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3bpftxtqx.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mxkgnrnw.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3hqfmqwxs.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3pqgrrbfd.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3vffjykwy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3npuxurea.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3ayxghtog.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3uxgeghwg.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3axzahrja.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3rwtylqgt.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3vuetumud.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3xcsqzdoa.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ayhrjbni.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3boletuoh.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3mmxlsghk.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3rzefiaym.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3pzfiogxn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3qoutavmr.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3aagwgnmt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3gbqczlrz.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3cgtxcgow.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3wfrzgnnc.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3gdribxxo.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3fbqvhmhy.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3ypbjhqlz.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3reglmwzz.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3iamzqxax.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3ncyfpffk.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ihgtsmsv.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3hspqgpxl.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3lkyyhvvy.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3cizfixaw.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3qqcwkasn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3htgixnzs.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3ydojbyij.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3ndvvvfjr.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3gjgoygpg.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3wnamxejv.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3lqvbphzb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3pxlkpbrp.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3udlsjlkc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3snuxzvxl.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3ccstebmw.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3xbtkgcjt.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3omdccoym.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3mtkzoctp.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3bhklhace.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3khdxvjke.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3isigviez.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3itpycfbm.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3zdisirwm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3nfuihksy.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3jzdiaqtz.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3duyerjmv.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3aomonlaf.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3uytxmujf.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kuyhvxot.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3xefoltxs.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wthgefkh.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3dnwyduhq.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3btxbmvnc.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3wuuvscjp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3coofcsnm.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3ezfmuxnd.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3tkkqnpmq.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3ttfgozjg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rkfglogw.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3tjpmdqxz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3wstjfunq.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3pagawmbi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3yqkriapw.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3igijwxeb.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3mxuflfxz.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3sisueeko.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3sxudvrqs.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3yhtmybga.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3vxlnfpta.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3elulyupz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3jbnoghke.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3nucqhtwd.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3csltwjzl.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3vntlaker.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3zaddvcvg.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3wqcrzvkn.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3pufzmbhc.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3prjruvbh.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3neckkgtt.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3fszjvdku.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3ufjdifdm.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3pzkpnzoh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3vtjzaash.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3enahlkyz.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3bgzyojqf.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3rdxpkqer.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3nrnoblhn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3zisizuqy.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3bqgaeusn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ogzlcjyv.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3cjndyrwt.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3tqlznjqo.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3pqaowhvi.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3zltgogza.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3knjwbwky.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3sikixozg.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3wtrxcarp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3swokfesk.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3ryryohbd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tzjtsufy.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3mshwhwzm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3hbfdqmrd.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3dnbzwmvi.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3eeapkchp.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3pxkiebgm.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3bzsocqcd.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3zqbphdva.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3wiqkcmdt.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3gfqxitps.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3dxojsouk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3usubanvt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3radnwlxv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fpvusndw.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3axydxapv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3lnehmdhr.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3xfbxpqwb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3nboifljb.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3wcswwike.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3kjvgjouv.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3pishezrs.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3rujnqqoy.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3rwjcldap.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3bqgdlezn.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3rrytxuxi.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3gdnpfebz.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3jzwlqcqg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3uhaptfly.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3saqmeluc.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3gnyvyyox.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3mupulkqo.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3kijasfjf.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3cbunmdaj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3moczusut.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3gpjmdqmo.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3clhwjfef.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3vipeofcb.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zqxeldag.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3rssqsupl.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bbmmimef.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3oczslrnc.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3fdeiydkl.html


<!-- 参考信息 -->