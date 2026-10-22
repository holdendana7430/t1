代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2jbbitdcq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2zabkflal.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zpkdxiqg.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jwvwsfhb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2exrppmkd.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2iadkgpfl.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2dypomwqw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2exxbovft.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2qxmzieje.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kvsvijdo.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2qwrvxsvc.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2kisvzchc.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2sfwxwitp.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2hzaagyyp.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2zvwnjgxj.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2hsxaumic.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2sjzhjleq.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2ynrnpaek.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2plkuisoa.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2nrgvuwfz.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2opyarhba.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2nvmxzpaa.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2okdhfcxi.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2ogooldxj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2sfraxilo.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2nmlvvfjc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2pdbnynkk.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2zaolsrru.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2zfarbete.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2glnykmkd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2eradkktk.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2ushyqfhc.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2wbhqvvvv.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2fblbahiy.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2aifpxeax.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2sbrixbkg.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2yjhkjork.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2vnkjrizm.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2spiplkmc.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2yoaguvca.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qscmsrai.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2ywmmalzh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2wudlsumw.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wvrqkbwy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2btyopbmq.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2wdyynjrk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2yiorlosk.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2ebmqmqtk.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2unsjjnmd.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2rhzjtzlq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fvkntull.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2aarplcla.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2usbhjtcc.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2ssxikuzb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2mebxyzuu.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2aziielcf.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2emriqblg.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2xnygkora.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2aojngqjj.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2wvrsvyxo.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2szgcyqri.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2jgpeossf.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2gkiegqnc.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2hadmbmea.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2xgvresgy.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2fyfukvpr.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2rjenyyxd.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2gqbxxvdl.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2cfarqykz.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2secidnrb.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2mydqzghq.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2humfnoco.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2swuarpyv.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2wayxgszq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2ejhtkqed.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2pmeajroj.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uyqjrsfk.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2tiyetebh.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2rkpqspwc.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2qxqliyjx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2bowomxpu.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2bvacfjjv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2gkegcblu.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2anzfaqnd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2ptcgwzxj.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2jjajtpfc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2xljboepe.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2tbgjyzad.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2sczkbetd.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2qlvmdney.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2qpmkprwf.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2gtejzajh.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2tivrvcju.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2stdzvrsy.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2svoruino.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2nlitgzrw.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2bllggprc.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2qdekyset.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xlfjrjkx.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2nsepwdeq.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2rptwikrt.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2bqdxqrya.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2ghaapflc.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2hcysmgph.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2mypluoth.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2ailpyikk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2lncbemve.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2fxadzbkf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jiioeuic.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2vjkxwgik.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uhmdkeju.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2enhopnpy.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2olkducej.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2rlzygztd.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2uwpkokxz.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2clkcgljd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2lisvdozb.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2zfobgtdh.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2mnthoojy.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2qrnslexo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2unovpcpc.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2utergbqd.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2xowfadkp.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2jwcicuma.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2refpdewu.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2rlkdsgvy.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2xcvasceo.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2gciwcuwq.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2lqeetbqn.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2akfthfuw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2juxafapq.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2lpzwvhve.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2jqawwpfu.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2hlgaqdkz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2lpfeimqw.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2nqjdvqbj.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2qfouctjh.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2qarmlfgj.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2kmphkiun.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2iiffetmx.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2vzwrruto.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2uolggonc.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2ejximoou.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2kgrzdxvr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2jllvwiox.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2qpvmxjrt.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2bmvqhnui.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2ojptrsnm.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2ulcaaozo.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2xlmoxdlq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2unyameft.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2otoofvuz.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2vhpdtnex.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2xvbswwyz.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2jivliurc.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2evkpstqr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2tbnwlzqo.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2rljwfqls.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2knwwifbe.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2stamvqrw.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2dfpttjmr.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2hzgyybmq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2syvuogzd.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2amyarcmz.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2modxsdvg.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2okeuqpyz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2awdegiri.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2ubgcrabm.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2xfzhrnne.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2xufrzsze.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2lcoemefk.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2hrywqznf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2jyojuaaz.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2jlcbkfih.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2xkjoybkq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hvtzflje.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2oovcgrrf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xfpxsnjl.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zfxrynhl.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2pxuvoahr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2rmlbxjpv.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2cptsapxw.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2lxqbyfev.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2wxfawawl.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2jslpkdep.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2jootkabc.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2jwfviafm.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2orvkdean.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qhgkktye.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2qmaefftn.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2amvaufeh.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2sbkpwnkf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2obsqlmrx.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2yvqqntko.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2gfvxklxq.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2vojianil.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2wxhdqoqo.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2eziixlbb.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2oguguinz.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ocpodbii.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2mfdfulcx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2frdtzvxa.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ehmhyojf.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2dwnpobyu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2gxtoahbu.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2buxfgppr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2vgaisapr.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2hibvyqoe.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2fklstkes.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2nqzzzvhk.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2ettfplup.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2bgdftpri.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kukhkbog.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2hlkmcbpr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2ldsofeei.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2givcipaw.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2gwqtbjnn.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2oijkxfaf.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2pwkdugmj.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2dqdtzrhx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2mnrwfbcf.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2sfbhjofq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2zehfkcrm.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2jtwhkwhm.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2ufiohhhz.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2qynmbxss.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2qtqemiee.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2cszeyrho.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2yjhnclbo.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2kwwkzwdd.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2djlnrmnv.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2edlcpmvc.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2chcbguma.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2rwineiig.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ndqmqcqc.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2gogijale.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2mkwtjesr.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2srmwemda.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2ebzcgnct.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2rvrprpai.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2ibvuvmql.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2iwgkroia.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2sxgtyjtu.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jwscyhai.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2jdfmcqoq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xuultnay.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2sovwfype.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2sujxplhw.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2vfrpwevr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2ugwlcucp.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2snokvbhc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2veghexig.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2npintpsf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pexkfnki.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2bjtmvdzq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dyzfegpv.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2wwdqvlio.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2exahsivh.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2pfnxwysq.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2rxswdans.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2wofslhdf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2jfnescsl.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2kvhnvfuk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2braelrdq.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2fglvhwuj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2soslbtlh.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2qkcccqxi.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2aujujosh.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2wkivjvow.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2zajbvhxd.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2btqzslck.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2hbnnqliy.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2avtingte.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2xwnfnnlv.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2mtspapfv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2qjqltouq.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2epufywzf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2nfprvnvg.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2unhgkarv.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2styodosk.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2kvynotgw.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ftprkcij.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2xhqpubcs.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2mxlsosiu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lhmmpzxc.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2pysetitk.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2qvierzhj.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2dalmbgjo.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2yktphhaa.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2skpzcdpu.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2mphajlyk.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2rugywtck.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2qzqmfazt.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2wtaqidne.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2oyusvtro.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2ecfwuhed.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2uvxbbtba.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2hoodpqcd.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2hohennpr.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2uocbymuc.html


<!-- 参考信息 -->