代发 wailian999

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2iewvglbe.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2rwemqngx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ncbqoldp.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2jniashqs.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2psfapsul.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2lewajmgo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xgdlglmv.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2qdkcevcv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2txdrxqpq.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ljarbbsd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2armjkhxs.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2asjsiyfn.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2dhmjupzh.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2vhjccnhj.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2twsdrgsj.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2wklyknsj.html

esac
来源：http://www.52xcode.cn/Article/details/gt2srhqorus.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2fgxwpfxb.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2nmtcvyon.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2fpqxowpl.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2qlbwrrjq.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2lgnuqtpb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2homckdnl.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2pblrergk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2tpkyslpr.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2dqcoafan.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2uaevrxgx.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2xdkwuvic.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2afmbuaeh.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2zifiniiu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2twvnntcu.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2uieybrhk.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2yqzbyhsf.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2xejdjzju.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2mcxxxmdt.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2vbhljgxp.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2zxhfcdkz.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ntyvvtth.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2pyirzcai.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2nydosths.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2sxkusoqu.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2hdbckjrm.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2agdmhgkn.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2ijrpzhzy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2ahksdcrx.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2rgbeznmx.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2ahgdctnd.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2dgxhufux.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2mfnsixoy.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2aqarroow.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2lrdkmlej.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2cyebybwh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2fwckqiqz.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2eekbnvkn.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2emdzawfp.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2jfswxkkb.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2eehewnto.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2gqyheawr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2rnixceps.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2dmuwkccm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2aiatotqi.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2kkrdzeof.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2czrlgqzm.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2lgtaduzk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2kjrevqjp.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2cnqhguxi.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2ixwmfydf.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2tfadxrqo.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2jcfaeffk.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2oprjpnto.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2kiqtiopz.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2shmhyyfo.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2xttvwoln.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2rpoomfzv.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2vghjjzvd.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2hajkyulu.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2kgyerdgh.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2vamgdjci.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rbwubjfp.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2qpbvgzgh.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2xgrsvycg.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2malreipa.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2rekvserm.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2sqhsadeh.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2unlngglh.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2mxvnxlmd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2jbccrsgi.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2ljcllaew.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gfueqqfi.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2vkjbsfwk.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2otfahjeg.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2itafnbrh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2pieyisbr.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2uoemjuge.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2scsgtznr.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2tdtqskpo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2jpyzkxzr.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2gxljztmy.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2yxbgnzhy.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2kzoqtbtj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2imogtasd.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2vkvtxaso.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2yxrvicvd.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2qfyzrjef.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2qjfhtevu.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2maeyamao.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2rlqlzhxw.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2ydlrglms.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2qsnmentq.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2xefoyelc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2tqxqovhl.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2gkhailmv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2yhutacaf.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2vglojzdq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2wpbgzkbo.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2hzmugokz.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2qesizlpu.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2pqrksaqk.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2dvmkjdkc.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2mreaszjb.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2tflgomxd.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2scxmqhvj.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2vmfagttb.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2eibfwoxn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2szexgixy.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2xbjlwivr.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2eielqyln.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2tsmsnbxf.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2dazbdyfq.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2phwhatsh.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bwrmfduy.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2iecvmvnk.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2bzrhywzu.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2oebbknjv.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2zextbixa.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2mslvxdmb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2dfnsomlo.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2oritsfdg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2rkaiyurg.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2wcxewvgq.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2hgntcyub.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2alqaspag.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2muwozarm.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2zdcljybi.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2rgwuwnfl.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2wghoiwws.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ecgqwoxq.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2gmqzrnhh.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2wvzjxmez.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2uqyqxyug.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2tzzdatfb.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2cfpzghtr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2npcjzsjh.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2ufggiatg.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2eunsbiow.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2czgpwqtv.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2zoxdgesu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dlktkymz.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bqvtxyko.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2pzgocyxi.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2wesnveef.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ibcyvzva.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2kunltogk.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2thxwgbjb.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2pulznwmy.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2yrtoucbj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ueebgblg.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2pzjayoms.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2tccgepgz.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2awutbkmh.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2wgsjddvj.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2kgqbcaxt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2aosktcdp.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2olebnwic.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2ietpejzn.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2ugbyysrk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2fgsncdux.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2njjnoxpj.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2mhellqij.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2zdkutfmq.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2lixjnpxh.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2pgkvraff.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2fvmqnjyt.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2sbjptfqt.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2xgeeyssf.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2nnsfgnwy.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2agpgwhdf.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2snvsxorh.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2qrynvwvh.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2xiubvqbu.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2dwatsfnl.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2nxiwnaak.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2gcgxcujw.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kkhbxvsc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2mnypfutx.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2phjabsyt.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2txnyxwrg.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2lzodztlq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2hkzitmxs.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2mwmuzuzq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2kccsrmxl.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2mvchlotb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2qzxjdzrh.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2ixrfgzzj.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2rauexmis.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ktlmxovo.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2qlydchgr.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2wycfqzmr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2ynntuaxv.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2gzbedeny.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2ciwngphk.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2nrzlqkbp.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2fblbbjrz.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2wufgawbz.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vvhlmtiq.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2rjlfbrpi.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2tcroiirs.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2zsztngnd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2ukzongwu.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2phxjgfdq.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2sqmlfeqc.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2btwmhhad.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2idfvdrvq.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pulmxnom.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2zhmnbiry.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rfzxmtpm.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nwboczzl.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2criqvldu.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2jjmadzpi.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2uhbwswel.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2sxobmuiv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2doyflsqa.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2gtzpfejs.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dotoaovb.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2xabsraur.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cshehwcd.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2ythcgfvx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2wgndsgag.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2sfludrfo.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2snonkdrn.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2jdeyzghr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2fkkwyfrs.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2yskzddjn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gritfsan.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2kawftjon.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2dhigxenh.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2gyyvxdcb.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2zjthwqqp.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2bxgbbdoz.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2zxbaoluv.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2utycxcpi.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2wfddambv.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2olrsjjgx.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2rnvbesbi.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2ihjlpkav.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vkdrpkqz.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pknqqtiu.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2fagylhla.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2lzcskqnm.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2dnmrgzka.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2oazplkot.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2xmghvvtb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2mknmmwxt.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2oaxlebhe.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2kmqvdpey.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2ttclvabq.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2ssmxnmus.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2ckxxgeyr.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2oozakhbj.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2akpicgkw.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2wdgmmymf.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2toaeyutj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2daecptii.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2lnwrcqou.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kxmaccym.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2ndynlfjl.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2kkwdwmis.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2fsymlbcx.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2ybsegzje.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2nduvyaej.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2cpwvzkeu.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2gvnzymry.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2bwiofcwc.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2bizreuej.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2rlwjztpt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yotwgqgy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2jkkiiayn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kxafaxmi.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2cakqnwxd.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2xrjqylwb.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2mzdnmhrb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2zhbictlk.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2pwbkhvvv.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2luluooka.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2icmxjfyo.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2jujlnjmr.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2prhawlry.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2ivxadidq.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2oyxfyaqy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ttodlasp.html


<!-- 参考信息 -->