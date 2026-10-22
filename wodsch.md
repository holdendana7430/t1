代发 wailian999

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2pjmaqkkx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2djpqeecp.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2wbpuxjrg.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2cokmphga.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2qxhwjvqw.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2naupdezw.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2igqknhjv.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2ahbcwssp.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2jsirwxjt.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2oclrnyvy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2fflhodbs.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2rfdndnsd.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2meirxhyz.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2pwypwaan.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2tlhgkyoa.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2lrihzjmp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xxqqrxoj.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2dcppmcbv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2oabaqojy.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2jzxajehl.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2kvptasto.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2hjbxwesd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jezqcjji.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2ahopnfwt.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2zgmgreqh.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2trplkqyo.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ipetfrbx.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2kkdvoluo.html

esac
来源：http://www.52xcode.cn/Article/details/gt2naliawtp.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2snpdcjyb.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2bfsizjrg.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2vqifeqii.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rlffcsli.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2wrnaovkq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hfdcgozz.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ykekkuhs.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2fopchznh.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2irjedlbr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2oafvctzq.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2aasmflxj.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2ysxeoegb.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2treswefq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2qkwufzzo.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2wljicbtr.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2zwiqylxj.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2sohagrpa.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2rjywmzlo.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2mlhallqp.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2iotxdsef.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2oufhotph.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2foxszqlv.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ffojdtsw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2zkuadixl.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2bdarrpns.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2rjdlzvrz.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2izewbaic.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2ysjmldrn.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2kpdjxivr.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2iesqfotm.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2wdlhjuxi.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ayxtwyha.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2puctnpap.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2uvkydwif.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2pepdrrlj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2pqrvwhdc.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2yubalkfz.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2lwkenvey.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2rkfmwfqu.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zrnfrzdv.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2rygmrayg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2pucmhwnq.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2vtdhvpiv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2jtfnhbbw.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2plvcmfgv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2cravrbvu.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2hgkzpxqs.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2vechytmb.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2rgyueaid.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2hsgvvzcb.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2wfcskytp.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2nwxkzttb.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2clhtajbv.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2pzahowhz.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2fxrtuayy.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2shwyyraz.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2jvmhbrxf.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2pevgtebx.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2misyalpd.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ywykdyca.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2ohfyqapl.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lmcjkxad.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2zshjrkpq.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2gpnkkamx.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2ovaaqyis.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2uvdxfdpq.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2aknrnivy.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2fluvzytb.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2vpvwnzye.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2etcylkxo.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2shbmfvzk.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bkjyrhyb.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2bararhby.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2htlvpmft.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2ofqzyuxl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2djoxzawb.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2yxbvmxgr.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2icpuvuta.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2qwrprzsz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2ouezzmyt.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2xzewaybd.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dgzbxcpj.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2wbqxxslp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2vjchlvkk.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2qavdbmya.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2gbewxsen.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2nokrgont.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2oyjubypi.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2bhjodiwl.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2wexcnzte.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2mcmmgann.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2rvfhnhgq.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2estvgsel.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2ffpkxlld.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xfjhiawc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2vcqulpol.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ubmcuuzu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2ukuzwzrv.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2iiqbizaw.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2uybwunzu.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2zzordndr.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2dxqwxced.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2jrifrrmm.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2imjtmnkl.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2lctnphxz.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2wgonzrln.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2mnkvxnkf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2yawrlnpd.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ujrgzjvk.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2pzccsyqu.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2jnvrlbtu.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2qfkmrzxb.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2ldcncjhz.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2svfleseg.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2bqxgwuiv.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2kzptvjqv.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2vcvmgddz.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2ukxasndy.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2lbpvdtwq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2zhdiszzy.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2ultdfuri.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2cmgjzzfw.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2eulaoyci.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2wdlhyykx.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2wvhtjpjn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vtqdbroa.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2llllqqhi.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2htnejxze.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2gqsumcrd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2sftowtqg.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2hahhbobv.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2brappeew.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2iyhzckys.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2xjhmzzzt.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2reehkuip.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2ilcosuhr.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2hqtrtnsz.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2krohbccg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mlnylbcb.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2rlxqtmeb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xzrwuesl.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bjhjysmm.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2ybrylhak.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2ztmzoshw.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2amqpbzhb.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2nrgnfdij.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2xyhbrmcq.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2ufzjtxov.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2gsawzaba.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2sysxzuov.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2sjnzbnty.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2znxwowls.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2srryqaby.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2zhvoyoqj.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2gdterwfv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2dshqbmfb.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2yndsanid.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2dwuxckcm.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2nxnliusc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2fpuiukbq.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2imbtvndw.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2rmpkocrp.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2hxzajddt.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2qceripwo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2jyqebrbf.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2xmbriynp.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2pmetcoos.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2vyztoxfx.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2ulfbubfp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2arpaihfm.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2sulxpnvo.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2ljfgcjbw.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2zjxoawup.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2fyoeryah.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2jhwjtxhi.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rmhdzwfv.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oevdoolf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2wckixxft.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ckkdtnwo.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2honldqug.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2stjsujcy.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2nlwbbbom.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2ebsakxtn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2htlzzuzq.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2nuhaokrg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2zedxznob.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2uhmzbtjo.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2qznbvanv.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2illubzhp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2zsqfjzmg.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2skvrdcvp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2jfdzwphp.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2qmuxpqjm.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2vsmnznbg.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2uvusazss.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2qtjvckft.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2gvunhvbr.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qfhpvtfd.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2tpcyxjup.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2dhkxssyp.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2imowkmpe.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2lsycjpgx.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2hrblggmo.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2mszyaose.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2jcrsmbxk.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2cohxhpgi.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fzdatwnt.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2cirpsajk.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2mfnhgvdo.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bniceaxd.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2kxfbfyhp.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2lmfnamur.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ghgnuwpc.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2njdzvcta.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2tglirzak.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2mjzrogna.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vwhrruzt.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2iqxxcgwb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2coverxok.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2yoyyuzfu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2azrjking.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2bcsszzlg.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2iqxejzxj.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2sbcetuav.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2bjbweksd.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2cvjgihoz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2erxgbjcr.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ixkmoarx.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2cbmxbwvt.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2gdexvszm.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2nhqappdd.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2xcfobdgi.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2czktezyg.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2bgcdhcei.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqwjseai.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2utfnexiy.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2hsoqudnj.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2mezqdzvl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2owwyolau.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bgowpnyb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2gpdkweqh.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2olceyarf.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2umdxypwq.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2fmizktht.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2ybabxevk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2rlbtqpzf.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2uhyqcguy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mkcrhopt.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2vsellkty.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2cgyxnqql.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2kqqqsnls.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2jmrprfcc.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2kimjytox.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2ivbllnql.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2dnakwckp.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2dfywylwq.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2ohzymjza.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2bhrftoax.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2yejiawex.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2abcwsgde.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2fkfklhno.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2kojqowne.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2zkdpjqnv.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ftowirqx.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2plnzqfma.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2mnddwxtf.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2yxgvwxms.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2lkioucgu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zlzgxkzn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2vrzgqqqv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ardfecyp.html


<!-- 参考信息 -->