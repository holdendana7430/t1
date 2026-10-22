代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2dihhwdts.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2geeiyitl.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2sumegvru.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xotfchvg.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ltlqpilc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cuabrwsj.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2ohlzrgbe.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2yjfzqmts.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2cdrdjwuo.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2tgdhybsr.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2fichcpbi.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2fefxpoam.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2hmikklmc.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2ygbsxncf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2pqmvxfdb.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2lftajokr.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2fnrejjar.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2lbkirbsh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2liuuvbfz.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2jbtikfuc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2eorzchsg.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ioebqajy.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xudmuczu.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2gshpsjao.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2nnxqfpxt.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2uwptodjd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2hnrirvbp.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2wsexrcbb.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2qcabgiys.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2xhlfiefe.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2gbvfbuas.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2acemgnkb.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2dbfbvyvz.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2ylzezaxv.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2lxozatno.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2oasawbce.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2rvwxboag.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2ouvdwyzs.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2jvqzxzyx.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2sffnsjxg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2yllmrjbo.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2ewaksrah.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2xbiraovg.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2exvplbhp.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2igbbtzen.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2pugcgayq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2apgmdqhh.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2uwlmskeg.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2vbckkdsc.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2jbpwvrha.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2avqayboo.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2wovukoge.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2qgfhmreh.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2wywqplzz.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2cddqubfj.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2hepkqald.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2ypeyuqdy.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2nnjykshx.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2uaqpqcsv.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2scdtlhwl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2sprwiyws.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2jmxzjjwk.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2eyzuhnix.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2fqsvoput.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2lsyfrosj.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2vkluesnh.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2ehvgmugx.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2rsixaoex.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2vbaakuls.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2ozxixigq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2nklhbtun.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2eaczuvrv.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zihvljyn.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2pkupwbkz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2cbsrkoge.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2ahxoqsho.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2qusbtshc.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2ubrmijkh.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2dplywmdw.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2xvlpztwz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2aiihwhby.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2mnbiwkxo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2eubwykdc.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2mgrjityi.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2gwbnwtxz.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2xyjkebkw.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2iqfvuyju.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2gthyldja.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2kvqhbhzm.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2usslgind.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2rzzouvmf.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2ghkrszjy.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2fieljzvh.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2ridhklzh.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jsljkyuq.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2gdkbucma.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2lckudpaq.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2wbtwtvlq.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2dttugxcc.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2ttcksquh.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2azpkcyvn.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2lfgxfdbq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2idaofhqh.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2shstpjdn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2eavlcdny.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2mukmhhyn.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2bnfscqnk.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2izusnmxf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2xlzrkort.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2wqdbtlme.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2benhzxkc.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2zuaewjtw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2fpythrvl.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2briynigo.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vqkcdfwj.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2chgtmliz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2gagyzrqz.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2lbfjivay.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2vggdaezg.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2jsqamlam.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2lyrfledu.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2zpekhcca.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2awzlpwbw.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2itmtfffp.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2afgovqhs.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2sdoxwkkn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2wotvdphx.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ammzmpgg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2gzrethrq.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2wogvjsrx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2lnwyubmv.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2sdlxheet.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2msexocga.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2tqhdxzag.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2cfzkwduk.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2dlhtibva.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2lpfmhaxk.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2coasrhao.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2bjdzsllt.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2qpuotvmc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2xunufcrl.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2spvjzdxq.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2dqxqsoeg.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2hnefwgkj.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2mjqxijuj.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2flqmiblf.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2vyssahmj.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2oysfdbny.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2kqukefqk.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2qjhirmyx.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2gbtahdfr.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2bfsrybyp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2unyouywz.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2owtpjjdv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2payxfkww.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2luezwvpl.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2cxyxtydm.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2uwaewyzz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2fnzgyrki.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2vobpochi.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2atocanth.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2picnqedq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2jmdswrla.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2qjwnltat.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2wbhatyjh.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2fmspqwjq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2yidcwvgb.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2mtwsfitk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2fgosljkx.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2ieozeszp.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2tkxdkpce.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ninwmddg.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2rhmukegl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2umwajmes.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2siwellha.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2xxkftyfp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2felguocn.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2budmkvvo.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2tgqlxmlp.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2syvdtjqu.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2glkmbjxd.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2tmaeeocx.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2rowxjrbo.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2tkdwyetk.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2twsorgqc.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2mgqtklto.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2uuubgceh.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2fcrpdlsv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2lrigxdzo.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2etuuakci.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2dunyvfzc.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2ghnzhtix.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2hoanfjjs.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2lniknjvd.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2yedpfigy.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2gvbtmokq.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2timwdjeb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2dpjchnek.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2uyodwhuj.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ayavponj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2fgcralgh.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2wmoevevq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2ucyutnry.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2uwbtbszl.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2jcukyxtk.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2vqomwsmb.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2akepdhny.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2rzjxweyl.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nhprmlna.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2mvcotvfw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2lvfstfnp.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ppvyykwl.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2eohyvvbs.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2fziksdxy.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2urocuwgj.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2qoyvgsdb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2kpmiadcn.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2fuzonyla.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2iyzwxtml.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2hjvyclzf.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2kqdinjgh.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2xyljumbc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2rgqpjwxb.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2ixvupyoz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2vkvspkrh.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2iyncbvhy.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2wllvvyld.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2biywdasz.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2qanjfoxm.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2zvvkdpzm.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2gocpjxwt.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2znjzkech.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2ckpraodu.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2ewmhfdom.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2ssccwfvz.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2jzofxbjt.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2zoskpovk.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2jpgxjjsg.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2mdkvbonj.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ktsssuxm.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2mdsnwdng.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2wdgayuax.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hmlaetqr.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2jsuquzly.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2egtexzth.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qemlmixu.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2dsepktcu.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2krhexuwp.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2acmitcgz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2idpegfdo.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2azhpllxi.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2yjekubko.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2hmeeusgk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2aufsrgyg.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2nkatvayu.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ppgfgtqb.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2mdehdqkq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2eoezftep.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2phdbiamr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2wvxloabo.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2kwrqgjkf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2ipftzzwr.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2ftzgdklx.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2ejslyphw.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2watymjhx.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2twkrxfvn.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2ahggbebo.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2vmsrjzyr.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2aunbdjmc.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2idvofmre.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2atxnovau.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bgzjxlvc.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pgszgwqy.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2bpvuehts.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ohglrqmj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2cflsvknn.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ybwcgwom.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2qtipvahf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2lfmbgfme.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2iuvjxfha.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2rrmfprtn.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2tqwhhqqa.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2jxornccz.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2ddnokzia.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2uahyugmh.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2bqbzftpv.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2kpkhrlbt.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2qpilchew.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2bbmmhijq.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2fvcezqma.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ewbawyhj.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2nmqcjdum.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2engrieqk.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2ebtlpdqo.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2rmqdoyvu.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2jsjaixbf.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2dquvzjmi.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2svmqodus.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2vzedaffd.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2rflmlnkk.html


<!-- 参考信息 -->