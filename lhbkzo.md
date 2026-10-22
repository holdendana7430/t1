代发 wailian999

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2dznkuhbx.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2nhxdercc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2ulkccfcx.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2cbammtmr.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2bvtdhygh.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2qwuebmoc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ppfticxx.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2dfqjgzcl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2buavjgbf.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2piuznlct.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2hzcpzrwq.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2vjwdmnmh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2dwopcsbl.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2dgsgmbfe.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2hhewhwft.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2ctmnrvnt.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2czmjrbkh.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2fadshnlu.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2nycisuxn.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2tqzostbu.html

esac
来源：http://www.52xcode.cn/Article/details/gt2kcyhulyc.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2unfrjtje.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2ifbortjt.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2rbagvrhe.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zjpsseya.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2lqthnddi.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2hutxvcme.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rchepmwr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2enzozwae.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2gezzwdhl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2zeukkbiv.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2atdexzkn.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ahwxjnvy.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2drjblobl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2apvzrcsi.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2vdauarlw.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2obhfxmmk.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2xnaiiqjj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2sduvautk.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2xztpixpx.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2vocbsgsv.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2hpnnsndr.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2lmpjiggj.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2sszlausl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2kerrhdzv.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2iiunejbs.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2shewhetv.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2jxnauyvh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2jztsgeva.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2fhemytec.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2fnivzchs.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2alyibfxf.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2fpcazrps.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2hqjsilzy.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2agzqlvox.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2otrhgctp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2arqxyerz.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2phdnkcha.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2nbxxzcfu.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2eujupofr.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2rckznrqt.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2ksiwlwsf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2fudqkaek.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2uyghyeah.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2sdxhxboe.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2wtfpfrcm.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2joyeknwo.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2cedyxluj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2zylwwizp.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2vuaylpbs.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2mmclisif.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2lcjytrqp.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2zzctbxiq.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2jzmrcmyg.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2skjxwmlz.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2ejllzmnz.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2icbwtrqh.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2akjqdust.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2edsotexm.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2qprrysna.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2yiyooaci.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2bvscpgvy.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gqqoovzn.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2xdycxqin.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2zotdohbe.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2mlpyqnmn.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2tmujflgw.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2tzksgvgu.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2bnywhmfg.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2ktlncvsi.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2umrivaee.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2bqutbace.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ffphgxik.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2cteddrzu.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ahauaync.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2biilwzsn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2xmcdqcub.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2xtbxwwot.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qfdzrhgj.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2ieqxddgr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2ccjumeed.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2enrozsuo.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2veaghrvv.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2hjltxzby.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2ddszdsew.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2rwlcdsgr.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2uwqvhthz.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2jpijdojs.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2kcmdhwlf.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2xpsdggao.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2wyfqmvab.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2bnnntpmz.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2dpdnufuy.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2tufkwcyh.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2byuuooxl.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ekeaaxng.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2kilpsepd.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2jytsrpgw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2mrejfnyi.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2jacjxptj.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2koauxzfl.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2fmrjazjs.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2fhplnxxq.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2qbtmiuvy.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2yxoswzhc.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2snovbjcj.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2upivijke.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2shjmhxej.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2wroqajnr.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2ildujbyp.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2zkdjqsww.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2uuewsvtt.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2uhgamofn.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2yocudrcc.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2olhsezgy.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2hirkvigm.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2xrsoxicb.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2lwedaerv.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2xjvfelkl.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2einnstov.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2prdxnixc.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2rhxrhinn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2bkmnlsfe.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2ixjldlvo.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2shjtxmmv.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2cgaazvjp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2upngdsty.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2chaudbes.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2avnqaows.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2fxqcjhnu.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2slzgkxhl.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2lmdqypbg.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2ockfnpwv.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2fkylqmyf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2qwpveadc.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2pshzpoge.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2pvfpigmx.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2yogbppxd.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2dvnwbdnk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2adziexxz.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2lpqnbvmg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bsumibkc.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2uwigczwf.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2lwglbrgq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2gaitjrjw.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2zpcvelgg.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2okehzlyv.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2tktyoomo.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2clizmshb.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2newmvelc.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2ytniresy.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2yhuizeac.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2wggedvpp.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ztnqiilh.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2mryhcpkw.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2hzuxfxit.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2bmlayryv.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2tzerelvw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2gkbguezo.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2jjmivmvj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2bswhrucu.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2kpawzxeg.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2cjxwkvzs.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2wnjgalvc.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2cgqthnwn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2lprlbiwc.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2csgsflho.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2gdscjzun.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2oawlhzzd.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2aejxunrz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2ewvwlnyz.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2btoyvnsy.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2qcoobioh.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2fnjpmbhy.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2drsdinnx.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2bpeiyome.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2eguwcrjt.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hwqywhyy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2swdfceee.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2uzrvyreg.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2sbrnovss.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2kmlxbzjx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2bwtmxtgj.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2wjzzujru.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2jqiuxret.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2rbvllzov.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2smvchemu.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2jlyffdmt.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2ehjhgafy.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2hqsegkkh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2pyezafat.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2hxkpxeol.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2zuchtdkg.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2yztczufy.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2wumtwmnj.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2ffuvxwdc.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2xyrrvvgm.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2hrncisqv.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2uvxnwtkr.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2qzhcecyv.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2jczrnksz.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2qycyoued.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2tkxifwgt.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2mwctaquk.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2tckamzzl.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2thrtxsev.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2bibqrawa.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rucogxvo.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2npeemnrx.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bkfrgmln.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jbpgkvta.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2aoasvapn.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2yulqihie.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2ugugpylo.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2jwwdbfvr.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2xcnsdowm.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2ftlapfgl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lhmoukit.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2mjjhdqon.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2givyxega.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2qfddfcsj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2mublpjcl.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2agpuvnkb.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ejxaqklh.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2yrxmpscn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2yjbqygsi.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2buwxfadp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2cxakunpx.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2paegyefj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2xxedagoq.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2uesdhpbh.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2zcjzbvpi.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2powemkby.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2dfgarxgt.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2hfdfasgs.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2uejpedqk.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2mdvjhgcp.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2ciirkixe.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2lxfcsthz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2sfgyvzvu.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mbdrsrke.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2mxubwrkk.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2nwochtby.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2avlwwreq.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2fmprbiiq.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2amxranvb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2otvqybdg.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2befvjvdv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zowssjad.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2tvdsnwhd.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2mrojewge.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2cldiwwrb.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwrehdqi.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2xzubsdxz.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2itybzeyu.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2hdgxbbmr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2fvqlfatv.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ltdkdpxi.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2zaqtbjbg.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2zyezucwk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2afotctoo.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2kkpowloy.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2xdqtsloi.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2zumughlx.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2divsfixc.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2hdrgpbhc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2wgjulzzp.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2jtyfwsps.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2jgqcudgo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bbkmtxsv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2fadydbrc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vhzcqtup.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2eeblefvi.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ftlremhe.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2fvhleiob.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2gdcjdtsh.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2ihbofbsd.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2thxhgzqs.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2trpxulof.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2pzponqty.html


<!-- 参考信息 -->