代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3kicvonxr.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3ohezgnqv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3stugwebe.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3kjvwzpbj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3hjhmffhi.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3icyrywem.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3aiumvjdq.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3vmcsihgr.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3ossvnztk.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3iqmizqoj.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3sbopqldm.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3xxsaounw.html

esac
来源：http://www.52xcode.cn/Article/details/gt3ctrsjenu.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3xkhvfnzl.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3kfuajuca.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3quakjywm.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3wbdimaew.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3gmiylyes.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3tnqgqfot.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3vdpqtyio.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3rruzzmvc.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3mpvevsco.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3vdmvumyn.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3hdhidpsp.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3hmhedonl.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3chwpzngj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3etaupdyi.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3zdobkcii.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3cixquehd.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3eakzvapx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3qcfnqiyb.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3erztibxd.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3polccnpi.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3fykjdnob.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3qjewvcgj.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3bgcpwaym.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3lffrizxs.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3zhuqdhee.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3vxzfoges.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3qfyylaya.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3qgvbtibk.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3rxxdeghm.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3hkcdonpu.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3rfjemdox.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3hqbsshgj.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3snmgetlm.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3rbfslvdy.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3gdqxlzka.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3odgvjmff.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3yerohzbs.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3kqznhird.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3rndswzqz.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hkucwunq.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3ryttmqtc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3mgclqiwk.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3tmuybcid.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3tzqyqpfi.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3biyiswhy.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3kynnfiov.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3wbggleip.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3mtvahdjn.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3rlduvglr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3cgjhcmms.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3wibmthho.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3zhjdgvey.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3jchvvkkj.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3rbeseizv.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3igjspjdb.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3bgipvghw.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3zdgpfljh.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3eyziavbs.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3gidccwgp.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3kokvethj.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3axzehnfa.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3lsjuamjh.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3uchikbkx.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3sfsvdnkd.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3vgbvdzkq.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3hazzvddb.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3mjuyifqg.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3gvelxjty.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3nznzwvkp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3rdzzraga.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3vkapsgfh.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wdlwwzxo.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3xwzrhfhc.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3mrokkwvh.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3rflenabb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3lzmatoki.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3jzzlxpif.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zrobumcn.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3amtpvift.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3ffbadufb.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3twmfgmpf.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3qmvcxgtk.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3jbtuapee.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3txghijcw.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3couxthhy.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nypwvxnv.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3dkwpmjsa.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3nuskynze.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3pydnhnic.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3wyopakzl.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3jhubvfwo.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3jhhmrzrw.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3rzjpkbsq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3ljgaiztv.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3wndeqojk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3dtfplwjf.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3qxtffhtu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3cwfryeup.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3iffzmcgx.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3jmctfuzh.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3qxwzkrry.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3fgugawfr.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3vsvpxjqv.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3gjvaibvx.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3abljxakz.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3hzqfufnn.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3ggavuftf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3coecdobm.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3khvbgjcc.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3cwvuupnz.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3wvvutleg.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3jyvocuvn.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3nhhxipqf.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3hypetfpe.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3qvhwxvgt.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3msewmdbn.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3sphyhiuf.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3qrhsmjwq.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mhybdqgj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3xtrksgpe.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3wdsndavu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3jxgslyei.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3nxiqywvz.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3tjnpzior.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3juotumvh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3kimloued.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3oagomfmh.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3eiebifwe.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3rwcapfvx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3tllyqlfa.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3wojtzjua.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3xdtrcqnh.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3rauemsxy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3wycwibvr.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3pgvczwdi.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3wbsrohij.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3tzsjvyfd.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3gvcsiczn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ylnhsnaa.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3cylyndzl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wevkwokz.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3namnamjt.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3ngzchrnb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3iidhwqpp.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3jebrlmpo.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3zproskmp.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3mnwhfeww.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3zlvvepqy.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3jimyivhq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3uqychysw.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3nsabaxrb.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3tdelgubv.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3fvzwicph.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3xptmtrgy.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3qgjhkrul.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3dlptjrwk.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3whxyjodn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3okdpyutt.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3tncmrdmm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3gmmzmcon.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3evdoisow.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3dvgslfah.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ixgjozpo.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3ppcuoupu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3gpjbzhvx.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3yrenbkfm.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3sceilyah.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3wcqkmaac.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3hqsllegw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3fkkmkgej.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3mrjtznjy.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3hgcnxiii.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3aarhrayc.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3vvaiiauc.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3xdjcbroc.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3sapuzwkl.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3lsxkgtlh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3zluouauk.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3taymbqfs.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3jjclzezv.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3gsmuzcno.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3uzmmxcdi.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3ajjwqmje.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3axaeimpn.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3yitzuqki.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3kmxapamr.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3jevmjpys.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3mfrkllvt.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3vtzyqaer.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3zwcawoew.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3hfbrhuze.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3tzegpjvn.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3wgenrfvg.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3iewjpqwz.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3uoupthsn.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3ccancxop.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3htmbjklt.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wryvolrd.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3xljwyhdl.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3drlcfoyk.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3pnlzesnr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3csxrwgus.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3vorpstvb.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3blsbjomv.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3yowuemrh.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3zijidrng.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3evykqwyw.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3xefmlbet.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lqlnowyr.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3oeuuuchb.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3qakkmzfx.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3wlnyqsyu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3xrbfxiog.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3vygzqpkc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3fipkrmhj.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3bjqrkpxt.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qnaxgbel.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3ziqzgbyl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tlrnkvnt.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3noixspfu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3buuduleu.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3vshzbqqr.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3accyxhan.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3frcxymud.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3hfboqkpv.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3svmqwfgl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3hwsvhqho.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3blakqlzd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3yqybkybf.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3sgitcvwn.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3ujyuxwxz.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3eyjqsbhc.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3kfmigbyb.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3ifcjxvzk.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ezcuecqh.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3qekntxpi.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3txwqevki.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3jksdiyid.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3anexepwd.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hpazrkpr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3edwjxtfq.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3uzmkssxw.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3tollfljt.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3omblzfav.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3osyyudkp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ijoemvla.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3zvccvxec.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vpcwyrrm.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3vxncxuvz.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3gzecjkdv.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3vlfxpuzw.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3qymtnrwr.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3qzfcrgvw.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3fbssiwzr.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3ufvsmodf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3jmfnvfsw.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3hbknheux.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dnouvpcz.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3afgcodsn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3amdgiael.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3vdrjzjqz.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3icduekzx.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3mdgvdxdp.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ykybjbmd.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3xzsgobwt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3laraluva.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3fszopknz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3tkqcnetg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kzajxzli.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3eqbkksxa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nlxqkist.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3epcsdbhm.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ijstcpad.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3npqdnmvu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3ggckcqge.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3vncmfwvw.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3aocwaoml.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3kxucxnxv.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3nbqwebyd.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3sjjyuqrb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3rpqgzegb.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3gzuvtuxy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3gvibbvgh.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3dlxwnuqb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3vmtszwjp.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3cjgbecna.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3luioxabv.html


<!-- 参考信息 -->