代发 wailian999

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3mafiirly.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3bmctswvi.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3tlnqxhnl.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3xlzzzfov.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3ovtgnohq.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3pnvqkqid.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3wnbzvlou.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3zoibnufa.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3qxnkczfz.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3afoiuujd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jqscrhpf.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3jjdsuveh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3msbsescz.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3pibngcpq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3zkmvbttf.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3tfjlrbog.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3eeoplizm.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3pbztubas.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3yuwlzoas.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3plrnzrxj.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3pzavclyl.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3dxgtihcv.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ipnuebiq.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3naumrcuq.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ktrhpxdd.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3jxtsyhnr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gzgiuiga.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3oisgvjye.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3wfkxhvic.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3qweljszx.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3fkuxnmch.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3eyowgrkt.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3edwhabfx.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3ugkjzlfy.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zrybxcjk.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3gvxkpqot.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3mmdbbgoc.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3ybyrrmyq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3auxynxmp.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3eaxgvaxl.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3ptjpepdn.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3skgzirpx.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3eyveqztu.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3hrueevwe.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3cnwcpdvd.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3rhzodrhb.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3sneqmqjo.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3wlnychlf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3qhbeyvsl.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3nyqvzumg.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3vsjqahxd.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3txhydlzu.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3envwutru.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3lmcaqpni.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3vsklvjpm.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3arsrzqmj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3oujtqudy.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3gtpivwih.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3wcgwfpzy.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3mdfczkoz.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bjdvuulq.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3sfdpjuyq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3szgpxyif.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3yyvcdbqv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3pvztcimc.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3rdorcprk.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3svozwjfi.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3mqbrhzru.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3uttvyrmi.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3ngqhxbpp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3nlqgvauo.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3ijzbeqlp.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3iddcbckq.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3cmjcbyvs.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3ylauvpjg.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3ljlbwrjn.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3gxzzxjll.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3tmjyszkb.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3jqfudyhx.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3cixvtjan.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3wrcwihax.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3zszozwhi.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ryrebckh.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3bwbmtqqb.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3hczdjooz.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3tfedbhgu.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3dqmificn.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3mnvgehsr.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3bgwllstb.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3oiupwshd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3mxkbabmc.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3maiwodsn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3jmacvotc.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3bfenwbfz.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fyzmhvnh.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3agpfzhrt.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3qdybnpjv.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3grfsrolk.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ilonpsku.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3pyytoolx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3qcapcrmd.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3eqvzadyz.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3buzhgxuo.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3crxbzuuo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3ssqqdbzh.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3rewedaou.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3nvtetjcu.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3egmsdxak.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3rrcxehdf.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3ypexdwzb.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3oagnxzbt.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3znanmtda.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3gomgrdsw.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3rbzdawop.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3hypqmspb.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3fyfgkpid.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3qdhuxvey.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3sqxwbihz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3grwzhlya.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3itagceex.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3ascbxkve.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3ptaendqo.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3nxhjenlp.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3bmkoiylv.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3zitrgdbr.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3kaxzmnwb.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3qmtjgman.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3mazryuzy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3mivjbncf.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3eheaxyzs.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3tdjadftv.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3lcwwpmbl.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3cdzaupzu.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3syvgnfhh.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3givkhcbn.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3cvmkkicn.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3fjnatofq.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3nhbtshzi.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3axmgstzi.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3wreextev.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3qqtzayvw.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3zambfhrr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3iiayxaze.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3sjdkfpgq.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3fnunqgzv.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3wwrkfkmt.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3ijkcwrjf.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3fxcxbqoj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3gtflegha.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3yvzkzwja.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3eeyorbbx.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3jjvfcfkt.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3clletzjg.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3clefvotp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3arpphwis.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3sxnftamn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3nlzceoqr.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3ndwpdkpf.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3wyzlocpv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xxfabhvr.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3llkxuziy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3audksyjg.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ihmvorfd.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3syycrglx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3ojjipjbk.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3cetxoarp.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3nqsnqswu.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3pizoovaw.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3seckksan.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3ivgeigpo.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3zsidrdud.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3apbzhjar.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3ovxyvnjy.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3jpeoefxc.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3qwwsexsv.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3xdzaspjn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3logfugju.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3adyzhype.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3zeuxlbwm.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3smxvlmbj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3jtllgaey.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3pnhyhpoh.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3pgaqxmfo.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3zoskifeb.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3vjymcxmz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3cubztjdl.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3doykcxfr.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3njkixxyg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3xjpqxaog.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3fykjujfs.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3hwxhhxsy.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3gbdxqtcv.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3qzdxbtia.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3slgdbqnx.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3prbudjnl.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3qtgxbcif.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3shrgyxfh.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3oxwtkmqa.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3zwlgifep.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3cdfuhcwu.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3woalgxlf.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3uusrwwpb.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3mgywbkvu.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3llxpxagm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3jywmeuyl.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3nqcgjzka.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3ctcihozp.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3gzceutjj.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3qibnlbbb.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3effecedc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3mjgvebim.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3qetgjddt.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3qnisvgte.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3jpmqisbg.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3ypcxpzpp.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3ubygeddg.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3umuuaylu.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3hcsnteoi.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3kqixbdiw.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3nwipuxop.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3unkjawfc.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3eigkflje.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3jlqwkdox.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3whyqsyya.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3lhwnaajr.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3yzprfhfp.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3fnqjhqmx.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wiycnlch.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3vgbkbopl.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3peunpqmr.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ufoqtjbx.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3ecnextgo.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3vrrweoah.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vrbiurgu.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3wybuoxnx.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3vjhlsqdc.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3vytopcxe.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gomjshal.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3cwpdeynf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3srdzaopq.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3nggdmgao.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ydgkraoh.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3addumpmz.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3gnqabiyk.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3eyyjokxi.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3avbsmybk.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3uwvguzid.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3ooauletx.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ckcebcst.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3pwithhmm.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3mdtzpxnv.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3ooitikjf.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3rqjjvzgc.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ikpcjtck.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3pqcfwkju.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3xgpkrpgx.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3yngtluzp.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3hiowzbio.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3itlemnqp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uwalxjus.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ytfwijlk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3fskheein.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3klqiroxs.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3donbdfvc.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3dubizbkl.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3elfwdwoa.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3xvzefhiw.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3zmpqdvcn.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3pacwpjvw.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3nqusmlgb.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3tpmgsljn.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3mcrjtwnv.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3fpxsabqx.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3vttacjdt.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3ufrlqzjp.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3mtufoybm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3fctcnkbq.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3btwltobn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3uekigmhx.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3tyitofwb.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3dqnoweel.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3dupuzcvm.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3zqhvzoww.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3oupltsjv.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3cblxnrbg.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3xvwprgbk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3ubkfnxro.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3iubzihlu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3podfxlui.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3elgsdyyn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3cpkrhkpk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zjnfzuhe.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ehfcbspc.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3umegilnq.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3cxrsbmsd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3btboymcr.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3ibtskxdo.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3tlzxfnfl.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3aeroxsfs.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3dgaapxha.html


<!-- 参考信息 -->