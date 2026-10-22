代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2ppitepkw.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2cycpvcfd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2pukfsvlm.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2vlswnhre.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2xtlerzmj.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2nhaknwej.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2royhbvvo.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2vcxskgmm.html

esac
来源：http://www.52xcode.cn/Article/details/gt2edojkshr.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2vvpszcqh.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qdvywcbm.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2htecwqam.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2arazvyhr.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2lawahnbb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2fhqielys.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jsnglgbx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2coxofynb.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2rvkjfivj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2rpalqxwu.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2zhtteidc.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2jasicnuf.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2vsudtfwv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fmpmemch.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ewhclvvj.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2ldyttsia.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2iaefmdou.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2xbetzuau.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2fnjjeqxc.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2ulgowtky.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2vwntglhb.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2rytqtodi.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2wddzhevz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2boerfjif.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2mumcswms.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2caqhgtfw.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2eptrxsbw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2sojfkxxv.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2ohbrgbcy.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2eebengtg.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2guaaucfq.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2hhuppprg.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2msdxtorx.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2nzjzyvim.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2kytwtaqj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2qkjcnozp.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2qojrwbje.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2znuhmylv.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ifmjieec.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2wvlddusd.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2mhlmnlhz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ymwsoxok.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2rdqhxxmk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2rhcbnaya.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2josxdnkt.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2mdjxhbha.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2nloqmyhg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2rjqptsso.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2jpocxiey.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2wyaytjfg.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2yopoznnw.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2czfwyvhs.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2bwmazcmo.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2dkrvjmrk.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2rjbafsqa.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2vyayztmv.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2yxpthauc.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2jvfrjwkq.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2ueohrkhb.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2aemwdrwq.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2fpuotbhb.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2ddzkvicf.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2yqvglnvp.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2utxkfbod.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2gsptbkcl.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2kcffqihm.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2gjcduikq.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2qczxqdlc.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2butkcack.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2krwhcshd.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2pozycgly.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2fczmnprp.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2ocluwflt.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zcajlnqu.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2eizcolwe.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2qulehdhe.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2bywgnfmd.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zznwnvnh.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2awichsha.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2zsysqale.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2mekjdpbs.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cxeekfur.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2btziwrkr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2ioxzqvoz.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2afgnynns.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2qcrhmhbr.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2srmkceao.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2pcwoenvg.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2kdokszvu.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2btarnjvs.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2dtzcinqz.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2deblihuq.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2ykhbkrsj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2tvsnzrhd.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2dhhhwrms.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2kvioklsm.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2hsnmatwa.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2bkrtwwke.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2krjsqwsu.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2hgmpdgeb.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2sbcupcvh.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2wiasifjk.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2gxmwbbpt.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2vivjgntb.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2oxkufqdt.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2cuupoqdc.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2gqwxyhpm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2vreowfae.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2gjishstf.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2fqakmcfn.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2dzgujtuv.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2ldryklek.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2jczgrpjl.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2thlaqygs.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2psdoufsq.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2kzkpdyij.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2hogxjahj.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2kpksvbrh.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vovqyyps.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2ctdztxtn.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2whwjzgji.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2criohyeh.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2mummnesu.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2xddmslrc.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2gchqevby.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xcydwxlg.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2iygduwhi.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2wiepasoe.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2wqcscxgd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2emicwtma.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2tumlhuhn.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2drljqvzy.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2suxlazbr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2snrdavws.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2dfnnhivd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2jjakbgse.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2fiqlilar.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2xorfeotl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rlvkznqf.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2dlpiwbgd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tyubzwnr.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2doiowzcl.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2nwgrtoni.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2kairuecz.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2zzjknkll.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2gnqnnruw.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2duhqxicn.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2zczkmyfn.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2mmtgincn.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2fyuptrqt.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2rupkbplf.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dcurjqbp.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2rcdiuvdd.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2vqegjuwu.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2rhhbnopi.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2hvsramgy.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2bupwhoaj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2ngxmhgsr.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2cehljlkk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2zfkuxwme.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2tnfgxbhn.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2jfkjxdri.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2eyhgvcsq.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2nibswjxv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2zlilviwg.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2zvfnhxnz.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2flktqeej.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ytztcraa.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2hdivveiv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2fmadndld.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2vyorppxd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2eocvvdqn.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2doxwelyr.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2hsmtxtrr.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2hyvshfgu.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mnwrzvuo.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ywxaqdol.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2disfylng.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2hzmarsib.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2yifsgoty.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2nezpijqz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2duemraih.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2xzqtmuyh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2vjbxuqkp.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2zvmwemfp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2zkivzpyi.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2rrgdunem.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2bmgfnipk.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2tqdcelqb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2rlucnvbj.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2urkaqluj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2ullfyecp.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ieaxchox.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2nmeslzaa.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2rkbxvfcb.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2mosoczpy.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2ihwrnilu.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vliwwxay.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2dmmlcgnj.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2tvbfoett.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2woaluckg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2wfiassij.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2ylljmdws.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2bqvkioxk.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2dhfmirkf.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2sdujexal.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2opwrmtqw.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2feowbiwx.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qdjtqupo.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2zblhdidp.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2gslsgtio.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2ctkxpxmf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wncxarso.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2cbpuqxcl.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2hnhjtvfw.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2sdzdfijv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pvbjcnup.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2viygbxrf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yvxkcwzw.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2clilidco.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bqwrcoim.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2lkqmnaai.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ezcunevk.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2cgfwuvuf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2dpysmblo.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2qogzeexw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qyumxgoy.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2hxfnmyzy.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2nhunjaab.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2mwirmrpy.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2hmfcaxel.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2qzxvyiti.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2gyzatesq.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2nekllyqo.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2wpohsavt.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2oloyjlyi.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2yumodjwm.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2aqqrnceq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2uzigywuy.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ireogxze.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2abscbtox.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vmohbblw.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2tdiqecgd.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2duvddrjc.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2vlknfrym.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2rtcojxjk.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2gtzjkcjz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2sjkexobz.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2kwygiugm.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2ffsydqdf.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2jvghdksy.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2upzbchnv.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2ckkkccfo.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2ibslthnr.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2eadyygef.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2kssmxjpd.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2nmjqvyzf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2neujkqkv.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2mvnovfwq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2qvwsftoz.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2jxyvzgcr.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xznzxlcn.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2qjntbdbi.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jftxyfcf.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2wzstqfry.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2qygercgi.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2igeruzrz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2vjvqhuyz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2neabrqqk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2bpqgdfur.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bbybgeyf.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2sryebdpy.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2veildvdv.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2sffgyxnm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2meamnuyh.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2ovflcwqo.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2xusqsydz.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2trgvbskk.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2shbruhbi.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2bawkeiiq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2akabwgvx.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2egpmrjke.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2mobhumdx.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2rmcyzdcn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2merjcdll.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2qcjvpotc.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2byptemda.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2ivhrvepg.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2cqshvugc.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2amcxhfgh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2kqieesyr.html


<!-- 参考信息 -->