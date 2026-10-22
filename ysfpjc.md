代发 wailian999

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2xbtpkqgn.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2qxialpiq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2gmbnjzfm.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2poeslcmh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2lxysbcjf.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2bbvbeyot.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2euaaelpu.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2cnvtsveb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ozrgysoj.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2ntrmwymc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2hopybxcd.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2mswvkcfv.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2gjzseujc.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2xxdxthgz.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2kvpnfawn.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2wzdvqmvd.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2lvlmskxh.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2htvdsrbl.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wgkesphe.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2kqhyezov.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2jzptddye.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2xkpnagfp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2bpvwfslw.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ttlivptk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yfhinxgg.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2ysjamffo.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2glzcmhba.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2hijfngjj.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2pzpsbrdp.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2hvbhfuhq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2tyevkhwk.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2mkxoibnr.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ovdgwddp.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2jegutaxw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2phlvehqy.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2lpujzkgx.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2wsvhuomy.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2mznhnjhe.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2qgzujpsj.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2usdqqryr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2njtnfizi.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ucqxdnrn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2udhyzgqi.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2ywosvezy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2myyvkxia.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2xybdlnfn.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2uapbkddd.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2sjmxfext.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2yjbxgixz.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2ksvbrhdr.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2jcvkfpyn.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2womabaxz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2mmueavue.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2lzkggojk.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2sflcamoz.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2vorprxvu.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwfhwcnj.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2dujwmana.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2cuudlqtb.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2emuyokkj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2adtxalgk.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2fjjaqtaq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2wmtdhsfm.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2wigcrprl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2fhpkyeqq.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2fvbkduwz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2becmxcfu.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2sjedocta.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2btzrpzqr.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2ekqpkebv.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2xyutlkgx.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2qeyajlfn.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2jmaiaiat.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2caadjvcm.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2lodjtcnh.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2sknqyosn.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2lqxulusn.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2dpphswvz.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2kdlcjjqr.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2uiuvbslw.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2yjtmxrzj.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2qooxmxzl.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2sespzbzw.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2rnwriotu.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2qchtgpkq.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2siqlftgb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2pvjchram.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2sizxyrrw.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bhobghai.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2krjbbcnl.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2wpyxpdgj.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2aytkgrrw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2zwtfutcs.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2dnzytksw.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2skxtyxua.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2tphshcsz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2ebfovcku.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2pfkxeuqv.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2fhddwdxj.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2ctacgisl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2ysjqczxa.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2lzzkeqbf.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2crpthvva.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2ysocpfwp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2vzkqslzd.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2jistclco.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2ierfhyyf.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2ouvxtlhp.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2slnobuxo.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2talgadbq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2qmsbbduz.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zlbbkxoh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2uhaajymo.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ufonkrho.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2krhngnbw.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2lxxvuedj.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2qdmxsdzb.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2faqjxhfj.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2lcqftrpc.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2bsldnxak.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2ggcjvvjk.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2xdadnvas.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2cqdepufw.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2iuztrrgb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2riodbmrt.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2kphfapyf.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2nsdcchuj.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2kxyjluee.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2tokrrdfq.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2ldbxuyyc.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rnjtshiq.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2xlztdnfj.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2mfjidrwz.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2whhnwjhe.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2milktwzu.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2cflhxxmz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2etoywikv.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2nqlxktoz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2rvkuxruw.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2jkrmikuf.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2iozsuarv.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2begyjrxf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rhsfapoa.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2wrrbdpqy.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2mdvrrlfh.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2qfjghfwi.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2cydxujbd.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2zzuaiwlv.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2beppabrw.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2rcebacvn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2kdjmpozs.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2nxcvyolu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2bieaprqz.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2umndsgam.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2agvgqeov.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ciavajmn.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2qhbrswtt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ilnfnnle.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2sshnhkap.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2dancozei.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2vvwkjilw.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2cgrfvtak.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2dluvztai.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2ctzvivaa.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2zdrdcdxf.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2pouhhtpw.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2azraldsa.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2srjtlyrq.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2sfkntfue.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ccrfgzhq.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2cuovaydx.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2ygepjzhv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2pqercsdx.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2lipmdnoh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2gfuxtedh.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2pesavovq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2dojeqjcv.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2nynagfek.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2fnbvztdh.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2euzpkytj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2srexxrhz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2snxbdrsv.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2fimctfcm.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2pxhtrpjh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2nzgecsls.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2qoavgoqz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2oeswpcwq.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2mrapgynv.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2oieorvck.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2vzkulhqt.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2mevepckp.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2dkfsrfky.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xfzlwgal.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2xtojfnfb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2vnifegxy.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2eqrokkyz.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2xquakuwa.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2gmsjshek.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2qgcgfraj.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2rqoerdva.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ojcruvvv.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2ohlxnbzl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2yqnlgjyy.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2vijxeptp.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2dqcpnwhq.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2zfzzqoix.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2lfffwefc.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2idskpbyk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2tuquuyin.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2mpzgnhfx.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2esicjxuj.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2rtiittzc.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2lwvrghwk.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2kohwkhrc.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vngpdhgf.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2lghoqgwk.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2uajpnysv.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2vpnpbisb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2wmzpubbt.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2euyccype.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ksypsvsc.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2lgjwpvdc.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2zmplxyxf.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ustjiccq.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2kcbtfsec.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2qdfozlnn.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2besbrvim.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2jojwrrsu.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2bejhydkr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kboicfbf.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2xxxxgkpd.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2wzvmxnhe.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2xzdrhzis.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2uzxkahxk.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2ogcvyzap.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2wryfqerz.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2qyheuprr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2glrkyuwq.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2ogismagn.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2dimsjaei.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2zblyanbq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2pllsbgco.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2yzrtcviz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rnhklsbn.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ydsdsumb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2sjhdytxi.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2keeviwvg.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2ockqqxux.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2sjthzess.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2wpfdifsb.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2zonwbgiz.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2zderqbbm.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2cdivkvod.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2lvwiiebq.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2rwnstvbc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ztheozpc.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2kuhlfaim.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2strrdvyl.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2jgkxlxtk.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2hpdnynpf.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2tsmlnkby.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2bkumyxca.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2jpmpjekj.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2gljpvdgp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xwyihuud.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2csmwvufd.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2xycrrrox.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2xunbxxzx.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2coxxmsvi.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2nupubocv.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2dfkiynlg.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2tuokqklg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2iubxzqhg.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2qsflecjj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kfchmfrs.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2muubittp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2cjezgunm.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2jibxkyxy.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2qhylyfxp.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2svaawpdo.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jrthbmua.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2mlvffjvl.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2nwhxvuhk.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2bwrmlzhf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2lotbcvth.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cfpsrzbk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2vjpcrkei.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vmquarcj.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qvaftmpo.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xtculiji.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2wldtvpsm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2mirmqvvo.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2mjseslbi.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2slycczfu.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2dqiuhgya.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2ixvhlomw.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vaerghio.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2iiumvzum.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2trkshypi.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2cacyzgja.html


<!-- 参考信息 -->