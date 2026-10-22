代发 wailian999

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2ydywfplm.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2gledojqd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2aloylsld.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2qaazxjek.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2mteihhzd.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2kpjxqxqz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2uvziwfnp.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2rtwmrzxe.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2orteiwpm.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2ksumnsvr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2yneuxnnu.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2uhkcvzmz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2ktjmvdhz.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dafwgklv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2zmpyfzpb.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2kgubdrvh.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2kosomnpg.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2xquzxbkm.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2jhhfzquf.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ctadxbpj.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2mtwnlyjw.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2mpdildqg.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2qneyvauu.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2lqitezgr.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2olnutqrf.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2zddckhci.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xqgyatcq.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2otyprzdq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2fddbszrx.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2upbxtoki.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2uiogydju.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2stbdmgib.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2gzqguejs.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2slyiaitn.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2nlneitsq.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2dttquwqu.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2yrhptjoi.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2hrcrswkh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2bjjmznnp.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2hrkyejbg.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2etmfnfqv.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2gporslty.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2rfeicosz.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2mcrixuhx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2elzbnoxn.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2glgqxzoz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2wrmlzhyd.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2dmzaxhod.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2xydlqmdb.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2neomerpg.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2zstfameg.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2nsaycljr.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2oztifkrf.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2niddghpv.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2agxdinek.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ayzegvrg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2ewowoczt.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2ghdgdfto.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2hcmqbblj.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2swmznmaj.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2kjogqtkv.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2nopmxdsi.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2lpxxtnwx.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2jzkokryr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2pzyqgtdv.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2ldcidiye.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2skrjruwm.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2eromtcql.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2trcdbplw.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2bwxeqjjv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2qthnqoce.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2kqyevsqj.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2pymovvcq.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2uhwdyhyl.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2delsmtuf.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2tawlkjfu.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2wwitegoy.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2gmroaoob.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2gtyjvhuj.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2cgxtmxlt.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2tkvmfefz.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2qtbpcutv.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uyshbhvc.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2cjuatuba.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2ljlmmgwh.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2toddjqza.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2ckchqede.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2gpqmafhq.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2ixnbptuv.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2fkjkgqyq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2hsrphbvs.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2drywazhs.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uerkkdra.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2gemhdyps.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2lpxkjijj.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2qbnoinoh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2kwvvimth.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2tpzdrogw.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ktmieiuz.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2ffjjuoap.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2cvrkzvsx.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2mekzgswf.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2egphbotw.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2ygxwqwwo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2qpppgxeq.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2nnwxiplm.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2vgdmizws.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2rttzdsga.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2idsygrob.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2jsbaxofq.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2inklahoy.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2mywiwqiy.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2xcxagmfw.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2jfqahunz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2xxtwolhx.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xbityrqy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2omqrwotd.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ydqsfwry.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2xgoyrpfm.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2rdrxbbop.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2dwqyzstk.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2vjoluwja.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2orouxuxk.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2nxqdvqif.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2ylvifxbc.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2abzucjce.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2lxqqqovn.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2ihdgqnzo.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2xikjwcbr.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2ghxblgta.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2eifptmgr.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2xbihtvnf.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2facoxaiq.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2zjikooep.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2plmeuezt.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2yuidqfdy.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2asbsawkp.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2dejquyds.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2zvglqkih.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ginxmbjl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2kjblsswk.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2xkqppvcl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2rhyvxvkd.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2axyycmxu.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2alstlnso.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2mowwbqvf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vclokump.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2itvsfmhe.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2sbyqjreo.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2pgrxhbvh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2umzlzuyi.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2bigaohem.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2kiplgmpy.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2wbhnuwps.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2vbwycmmy.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2falseadd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2xvlgvqmi.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2copnsbfo.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2liwdslxp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yqabmaqs.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2apmyiobd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fqivbuwd.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mmzkumin.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2dlsyumlu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2bcbbfakf.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2yirvyrxw.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2wsdipahk.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2phfbguui.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2ovympxkz.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2ymqqizxd.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2tjiryvyz.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2dkxmosph.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2snixsiex.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2fimdxcoh.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2uruonmcc.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2jrwpwygf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2hajpnazn.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2aefplyyc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2xejuorjp.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2wdkqvazz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2lipldvoc.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2adrhyzfg.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2ahsrhhdq.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ajhragqd.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2asuwztyn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2nbxofism.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2mxmufgny.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2gndantyn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2zkpugdxi.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2tynraqrh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2iklojxxm.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2uwrocpha.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2edfjnqgl.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2aqcuypaj.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2pymyiujw.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2jfddlqmo.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vlwxkngh.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yahhycjd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2gxhzsqyq.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2arvewkrz.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2lgajvhkg.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2dedtwpsf.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2czqfbqwk.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2tcgfhvpq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2xtuzskcr.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2qijbvera.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2mpgdzmpi.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2dttmspop.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2lkuxbmgk.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2loheyjuy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2igakcszf.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2dmwbpkkh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2fgklomce.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2lplhfuff.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2bvqcuenf.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2nwyxfulv.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2dampfqke.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2esbgveye.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2jodgugdt.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2pbhvlvvv.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2lggrmmgi.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2ujvpdunl.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2tldguzbt.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2jvgnfdim.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ozgoeldg.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2jvrtzzeh.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2hhmspcic.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vaxxeegu.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2vrsnidhs.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhwujuya.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2ltehvyvf.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2cvspeibr.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2zxdsltnm.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2ayfqeyls.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2yfmmdoio.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2xrxftuic.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2mghkrblq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gadqevst.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2semqsdzm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lzuovvav.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2dluesqfr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2fdgexttp.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2dpwaccxj.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2nflxmkva.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2bxllmqmr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2zpwdmaro.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2tiqkbtac.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rrxrhhok.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2uemwrlgm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2biuciccl.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2hzehbqpa.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2vkgzwedz.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2lvsqrxhz.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2uihijuyf.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2jgjbexio.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2zqxctkgf.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2pxkoiwdh.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2kywjnxvn.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2diwkhrju.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2nzvqstjb.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rlmbuhmx.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2xlkvyemj.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2uhztkcay.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2ekuycuab.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2mvagaxrb.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2gdjewlui.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2pgppduzd.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2zofuvllk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2rkrxiwdg.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2pfpfktsy.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2yadpfscr.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2aijzovrs.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2pqadoypp.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2nqedezyc.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2fejcuvvt.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2ehlwgjcu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2vhqsnfgc.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2ekinwqur.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xvesycku.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2svmrebzk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2rxzysemp.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2iitvaihy.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2knmbffta.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2blrxfovi.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2bsfsjnyv.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2hqpwntdt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2wrqciymk.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2kxhjlgdn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ecnlgfjp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tkdvtsga.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2qiybgvby.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2resczrgp.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gtcvojla.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ukomddsy.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2oflvzkid.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2dplkwmym.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2mcjobywp.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2numovvky.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2mpxkgftk.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2lecztsqt.html


<!-- 参考信息 -->