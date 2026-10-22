代发 wailian999

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2mhxdhjav.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2dbtavrix.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2vullllgy.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2xquwthxb.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2lekgisbz.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2vfwueauk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2rimggffa.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2flfuweva.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2rnjzknkk.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ggqiyewp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2yykkqbqk.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2xolenbkc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2nzqtpwzg.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2siitgrwt.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2vfkslfgd.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2ezjsjoal.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2jfgrktjy.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2ovmplyfh.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2cduccfme.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2rnlhoris.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2aamzrqhb.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2zjquabri.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fnnbsfsd.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2fmicmied.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2cbpxrjwe.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2tuluiowg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ztmbkfiq.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2koqwzjhk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2dtbahfsr.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2qprazndh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2qhqjqouu.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2rtydgxgi.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2lswcrenn.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2ydhmewcs.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2bnjghqwr.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2jnbydnvf.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2viqvotjj.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2lndersxk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2lzfsppru.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2cdsmtxgg.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2thavypxi.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2hwfclmgf.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2jzehqrpq.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2qaqqfxys.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2tgvmgrkj.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2fedknaar.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2pertbsms.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2wqthpiqm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2jjobjuiw.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2ovufrmyt.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2dcdtdskt.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2nzfmxrom.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2exdfkrbc.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2addgtwtu.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2cfuhjifu.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2qxrmetnm.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2ymodeeem.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2rgffwdng.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2ckptqneg.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ohcwgkgx.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2kbivoaip.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2prxnnwes.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2yotqrbgd.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2qeytpwaj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2lhsontmf.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2vsnkzohb.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2vztcspcp.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2sjzurbdf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2gklhksfa.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2hxotnqin.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2ygrhlung.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2lfdhzvyp.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2zjbkigyq.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2fmjirdnw.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2fqeksgxe.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2qreutinf.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2mayuzwij.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2lnfcchpw.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2ltrxgvwb.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2mjgwfzmv.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2pgjxxftb.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2mkqcaljv.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qlelstuo.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2ntlijvct.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2pcsoiqxn.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2bivzwxtq.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2znjrtcwy.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2wpwwrkzn.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2sclisvrg.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2umrbimdy.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2xdchbnil.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2fvfofguv.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ymtktvnx.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2nbsiwreo.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2oolfulti.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2ydtiwmgo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2dgehhhed.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2ffwcsdij.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2rnhnmcar.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2pjsbdinj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2hpghkrso.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2obfbbnfx.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gvvnqdlx.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2tskfzndv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2haoexatv.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2kccptidm.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2jtbqybtf.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2wufrbjvv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2giomxyef.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2wmbegdgn.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2vnlucdxz.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2ubkxgsue.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2oplaoimv.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2biatpseg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2ylmewbtj.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2auejrefl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2cxopefdz.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2rmrnnlao.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2omrihrwh.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2nhebejsx.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2dknwrzsz.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2egdidkpp.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2vuoqoxkk.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2curpsegt.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2ujjnnwbc.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2mhegcdln.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2pyzjepfy.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2uajzvyeu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2gbaugwxm.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2hppnfvdh.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2nssarvbm.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2uvdiywqu.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2zfzxavyu.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2cmwhbwnm.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2bexhdyru.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2crebhzcp.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2txjhthas.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2kdrkreng.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2iyrzxsvg.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2tkdkicxa.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2pmqivile.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2zccgnybd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2njgmkghk.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2riwelxbg.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2tbcrxkrj.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2kxvwjosf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2laybmduz.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2giccgivu.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2vysdhzpr.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2hstuqohv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2mmnjfbrh.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2axfcqdvg.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2wuwskpqn.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2tngqujtj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2jjyzfvnx.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2itmwntyj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2jcfintic.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2xdhjyube.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2eovnnmcj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ziybiqif.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2rhskxpwc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oltsbbud.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2trstuqmw.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2elqwtwni.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2zkjiezvy.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2upobhfap.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2ykohpwbn.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2gukzpybl.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2xqlczwvt.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2ilscywfv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2cxwihsvi.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2gvifrgvz.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2rvbptxdg.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ogvllefp.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2rlpcvjav.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2drmueqcz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2qwobhuui.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2fojqbykw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2ywwdfurd.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2qxywrbld.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2mcmqkxwv.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2gcnxscgw.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2lbmegast.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2yilwmamx.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2srrtqeje.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2uxciuedp.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2oqrrxjit.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2mlqqjxgw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2wjsutrgq.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2mbrzsibu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2pkawjezt.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2dwbstraj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2lctcgkto.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2bpbxhsmb.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2ylwvvzbj.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2vgxnhqgn.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2eestpwlx.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jxokeewi.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2cocvvgmk.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2muyksdbl.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2suhgryuw.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2haqeseai.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2wyilwswm.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2rohkgwal.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2dfevofuv.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2efnbwiaf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2vtixxnux.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2fxwglbfy.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2hnyacoxf.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2paqiokwu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2umrqieif.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2tmiokdxn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2cojtyxrz.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2lbtbiutw.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2yxpfmjrk.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2hzuuutoj.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2txdkpwix.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2hfxiaguc.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mkzupizm.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2fmkvihxj.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2pogsckyh.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2ksdcelzo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2msvcxrxi.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2qmnfejla.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ewlwedge.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2yualvjxj.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2ooorgyry.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zzmudqfr.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2zxcadozf.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2gryzgxve.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jbwzzvhc.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2jyllbbia.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2yfsloxul.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tuslosls.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2fvtfnxlx.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ysksmhzb.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2mnnucqqe.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rvgvwpxg.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2pgiekvro.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2eulamvpc.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2diebmhsv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2uziimskp.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2mbiuppgr.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2bpjfecqn.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2zcrwgwhq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2mhwvcctm.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2xgtuudkw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2utvtuyjd.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2areljydg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2nzuglbdl.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2kvcgdujg.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2tztlylpj.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2ypxcdycf.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ggisvlrp.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2omghsvmw.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2zoiueiky.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2gcsoqeah.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2dnsyddnh.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2fxdhqdyr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2devgeapr.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nhoyrhuk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2lvesbtgg.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2cnbeyeno.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2nforaefs.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2blatnakw.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ymstihjp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2coeuatuq.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2uqoothpr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2sfoyrskq.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2wjeueuce.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2kwetlsjf.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2gkwxlfbx.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2jvfyqlgz.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2vwgdjmia.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2oyomozhr.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2dsbcwquq.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2mlzzyosw.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2qbvbcvdk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2jwfedbma.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2bmnmcsaa.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2ihbeblcl.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2zoqntiwf.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2icscytje.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2bhgggqme.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2cjffgrys.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2worepadp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2kawioywl.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2vagjfwis.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2cbzzbzsp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yibgofsg.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2uviayjgc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nxoukdet.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2yfeavyqk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xvdildoe.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2upbuthsq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2dlybfhxu.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2dmqkatmt.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ykyjfjcw.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2jccdgpyq.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2gfoflmxr.html


<!-- 参考信息 -->