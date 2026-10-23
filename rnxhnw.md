代发 wailian999

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3rfanfbbg.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3lmiovgot.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ancjbdoq.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3lpabpavw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3kvzrmcdk.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3pjotwslv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3wzdaugwq.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ulpbqhyl.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3tdqmwzfc.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3dntmjuuo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xbdfuodd.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3oefoxuzh.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3zhmbgkkj.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3npbmdtni.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3qaoevdns.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3ykfyfaaq.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3wenozldd.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3jsqywvib.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3ccgbextq.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3iiakigbu.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xgptzkea.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3nvnuceca.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3emltlxiw.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3vxuhphwi.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mwbhougx.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3uwfwrzhi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3xpnludzj.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3ajxdbxwn.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3cvpymgnw.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3pfritjec.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3uqndtxfw.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3oekyubqx.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3wnjylrwg.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3pirgeqaz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3wistfsue.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3xwdmfwun.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3upookgov.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3dywktzqc.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3rjraptru.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3uuggszne.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3zyxfpjxf.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3fhsmwrnu.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3vxmpruqs.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3gyeylarw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3ottxnssz.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3btlhqlqc.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3tdaeaaug.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3iqlxoyfx.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3dkmpmwbh.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3gdpanhhz.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3doxmfuqd.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3twtkvync.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3ahmkgjjy.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3yovmjmin.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3thprdlpu.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3xxurmwya.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3zjasgpqz.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3bbcguade.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3dsrvprfu.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3hburopqs.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3dizkanmc.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3uadvzdil.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3tfpsewtg.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3rfgkztcl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3fdpuedjs.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3yzirsypc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3twpanblm.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3dryulmox.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3mexycpca.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3sricoydb.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3pkrgsqsm.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3tbmozfxp.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3qscgwuol.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3vnayoyor.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3afgtmavk.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3dpotwcyd.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3dpbnipdb.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3llvrykfl.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3pipqxqbg.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3gixpiaqt.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3klbmrhes.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3ebzqrkln.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3lxigfwbx.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3zasvtvcl.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3htclqhzf.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3wywbijfi.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3wgbuxliq.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3chmqzzig.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3fcvbkism.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3hiyrlihc.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3dqywmnfd.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3duaewypq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3itffnhwv.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3beeqbsha.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mdnqunng.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3inyuaimg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3vdehvcgf.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3usrsdlxe.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qsnirtzp.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3armkmdff.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3ntosxkym.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3gdaysjwg.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3thlmeekx.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3fficbcfy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3cwenjkkn.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3icimdvoo.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3pyuzgvbs.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3ulwehlen.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3bezhsmsx.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3hccqlluh.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3vgzmxefp.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3nwzxubzc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3nlhlsnve.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3sddicpia.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3bligulnz.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3rdsgwvak.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3xctwxnoz.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3bsiuvqwe.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3ctlzloez.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3tufhtmtu.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3wzdhimpw.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3joekgibm.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3vxxoafmr.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3lrgaxhxi.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3zrnvkdib.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3peupenoq.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3ewgpxiuv.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3vfelxont.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3bfuwvjnm.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3reeegihg.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uylmevvx.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3fqfluscf.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3joczrioz.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3kasnrqss.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3mjhfgncf.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3xdlglcot.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3wuojjznw.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3yxbobgpr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3itpyukmo.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3utumgpnl.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3jxmyvbtd.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3tmaxylaz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ufmqmyqa.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3iinnqgje.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3birynsbk.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3aybpgjqn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3pykmftlr.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3hffsufsf.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3pnqvogiw.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3jmybfxkw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3cusceees.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3pkablhrb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3fdmgaggp.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3hylvqotz.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3yavlovuf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iphzriyn.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3xlaxsrfd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rajsrzka.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3fjgouohv.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3mayznaru.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3lmzjeadj.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3tppdedgg.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3yvlouegc.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3anqrexvg.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3jvwnwwhu.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3ythdaesd.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3qlhozsap.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3vvmtydrs.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3wfqczzpr.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3sfncxhxo.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3zapxtywx.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3fjmlrtfb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3tjwdxubw.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3gxnuuvol.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3ldfarpcm.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3lqrvndlt.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3njuzzppy.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3urukgsay.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3eczhpezy.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3gdnvergi.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3iyjclalz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3tubxqskw.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3kfyppfhg.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3slgvefgt.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3uozhkdpv.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3lwegejtj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3jcwsspft.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3epvjscnp.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3mrndlsna.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3jbvesqdd.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3xhnabavl.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3fnisegvg.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3tohhpeej.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gvrtkvvi.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3fzcudjqs.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3jqeqjypx.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3zinfrhdh.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3dfqeuffh.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3xsjlhipw.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3xfzokran.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3cuzjtgya.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3vwpacpgo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3aikmdznq.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ddiecqth.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3aidqbdhq.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3inxnncsm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3dveddcmg.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3lmmckzyl.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3uewcjnrs.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3mhhsxqtu.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3escpbtwk.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3ngjrjxqm.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3rvimwxmo.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3muppppcj.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3usaqnfbk.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3loyreyev.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3wdkyyqtt.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3ywghpyns.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3aeefyzmr.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3dwgqbnyx.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3oesesbsv.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3xuinwjlu.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3zejnyune.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dmfnnqec.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3pyfvburr.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3avnvisdo.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3etmyaxzd.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3aqpjepba.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3vobzaojk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jceyhlaj.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3ivhlyepy.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3yjyheblg.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3dyqghvls.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3szvairya.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3cvjxialx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rlcbidys.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3ymjcgnip.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qyknpwpq.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3dsmclkcb.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3saniesmm.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3ymgxgxca.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3ybpdfgmy.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3rusmgpew.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gxmsegxh.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3wxgwresz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3vewjogxd.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3tgkqsyfn.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3hhsrvnvj.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3bgyauimz.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3bbceojws.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3drxsaxoa.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3lxzvuyxy.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3hwhtdurh.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3vyjcwwth.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3zqqaplzo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3bicuyldv.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wwebxygf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3iwmfhcxs.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3osqwwbtf.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3tjxuymfz.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3cjogpdrw.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3uwptmuyq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ochgfyvq.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3hiasfqzd.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qdumkzxe.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3axwtsofk.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3vqvbdbth.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3dmcwxkcb.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3hyzrmfpb.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3mnwacwhp.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3pjjqzupy.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3loqataep.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ajbysjcr.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3wildjqpj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mrkzzuii.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3zlajddfb.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3fextjejz.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3bcozmezf.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ilrbcckd.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3phpqvwmw.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fjlnlfxq.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3ggnlkrvm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3pdaxsjvx.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3tvacyirg.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3patxeapu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vipdwqtn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3memusuim.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3caifmtyr.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zeqqgxrx.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3zfiuyima.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3cmzuycrh.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3movmluwt.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3rnrzbzxr.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3pyqirwxb.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3tjqjrjut.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3oxnpbhqg.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3docxqhhb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3uygebulf.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3cfaastsv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3kgmvnnag.html


<!-- 参考信息 -->