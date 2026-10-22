代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2apmpqmeu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2ynegovow.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pwdahkux.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2rlfezeux.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2qrgvaywf.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2ezbyktja.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2llkwhzsf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2toiipsvb.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2cgxwzlgu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oohrhhxm.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2cmjtchjc.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2cviizrwz.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2uqchkplc.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2gtaboeph.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2dyaeeaeb.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2camkjjus.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2iwxglecc.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2pfnjhzgp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2fyrrfpnj.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2idlabavv.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2srkogqmu.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2yezlhdjy.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2pcnsostn.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2wgpwcgiw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2prrjgnwm.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2yksbsseg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2yzjvvkjg.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2laivmbcg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2gzvgjyce.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hldwxyhe.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2rmvvcujw.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2dfkmzgjo.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2mcgfyajm.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2amntqeva.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2qclluikx.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2xcjlwccv.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2idextkcc.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2itllbkqi.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ekgxrlvi.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2rjfwcplz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cegrojbo.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2uapxwcin.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2lyutegfg.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xswnqkpl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2ntgkzrqp.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2zgtdngne.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2okcoovqr.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2dkxqylmb.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2pocoemyt.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2erzugean.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2slmvgkbw.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2jzqembci.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2pnqukkcr.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2qplrvzjn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2yndwlxzv.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ciizhgkc.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2ccsjjrag.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2kuprnehr.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2qxxelpsj.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2taixbpti.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2srjlcsxb.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2kvpysrtd.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2xemuctfs.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2gxmgtcdf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2nmxmfbus.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2ijwliniy.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2jhxdctct.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2voukrzzq.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2tmzqkkst.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2qawsiejl.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2womljbsg.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2cocnznbt.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2twoasxcb.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2twozgrnj.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2nnvdfpba.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2rvbugbao.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2wmhrtogu.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2zmigsirw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2gtmjqhbm.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2aadjaoly.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2tjflzchs.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2jtvixaui.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2yfwdggjk.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2wmsmpdxa.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2alqhbqwu.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2kcaxdgfr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2lvsggqcj.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2xehqapmx.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2xyufhshi.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2dcuauemw.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2opxqcrzg.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2rtfflrus.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2azyivuwm.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2jfokoiab.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2cvutwvym.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2scubmhwr.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ttuaebgp.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2nchqdjvz.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2mchrehrk.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2ffobqlpj.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2avuhqote.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2autrvmcy.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2shvhybxu.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2xxdmbwau.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2mltiqiwk.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2hvvudclw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2vdxvlamx.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2ofbmutrb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hqvizdoj.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2kdefhhqx.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qxxemqrq.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2cxasgplp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2gxtmwbio.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2gpipqpml.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2mrxbiiti.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2qehymgtj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2kfecbgsx.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2jqrunkkr.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yqsyjsmm.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2spfokxfw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2neejzvsb.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2uohetwwg.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2nuyqnhti.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2slicutvt.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2npqfigxn.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2hteigsha.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2vmeeqioq.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2akhrgzjm.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2oiczkybq.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2mhalfcxv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2ygepgfek.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2jcnshjhg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2yonincni.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2nzdpywgx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2lnszoski.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2ltjbvkmw.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2gbuvkwdn.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2vcnrvuic.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2mlpqmhmw.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2echuanxu.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2agdhtmbi.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2jkabmeeu.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2ejjhzfvb.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2mfodpkcn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2alehcnro.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2idpvszed.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2vbnvjdla.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2dydheofw.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2qvwzqebg.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2fkokuldu.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2rkndlivr.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2wbdctmow.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2urdmkkrh.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2lzgsqgsd.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2mwnmdpli.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2worvzsad.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2kcdsjaaz.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2tycagcda.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ykmrkcvu.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2bdeoxwzf.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2dzxrwmzu.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2qavwuiub.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2fvtcseom.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2nhvjxnwa.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2ypqdxwco.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2nptolywx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ympczdqi.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2nadhxkks.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2vssdofzu.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2lpkiatvv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2tilxxmkd.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2zgqdgvvh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2teachopc.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2oajdupiw.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2jrdousoq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dsniaqza.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2cjensxfo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dqyclnsg.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kdxvxvnz.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2hacfhnke.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2ikvpxnff.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ztlpwaez.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2buwsugon.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2oktmxxoc.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2rrqcpznv.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2wowuvwpv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2axcecuyt.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2gfoqnzvi.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lsxwohtr.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2qfqcyroe.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2emhxztcj.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2pvmcdesl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2auwpptdo.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2hnkvfhmn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2telebeqp.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2bauywjei.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2zfgdsndn.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2esmnfknx.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2wlsiolfm.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2szkqautz.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2dbxqelko.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2opyygxoh.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2hgvreqab.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2gvcymvxz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2dotdfqzy.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2kulajwhy.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2qqthgbyk.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2iczhbsui.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2ujqnvnic.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2fgcyiefn.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2vvrpefju.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2vqznpyol.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dodnoniv.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2thqtuqlu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2ykfoecet.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2tdntqhfv.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2gjfjuahe.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2nxnrqblb.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2fxogplcg.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2rqsxjnki.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2vmjobxmh.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2rokbkowb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2pqhetsoc.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2xxfitfmi.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2phnzxolx.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2ffxutkwq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2qbktbqyh.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2ccbbqdzn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2cymndpvr.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2qonbsjjk.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2gzoyuxvb.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2pkvkdsoz.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2jombwtjg.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2ghejgwte.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2icduxatq.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2hgagkusm.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2apjucbrh.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2wdjwaghp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2sslqkepc.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2ultjopef.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2upqejlgz.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2dypmdpri.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2ywnguiua.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xvpmtaeb.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2umumqjud.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2kejqmkbg.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2jsxmhhsn.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2onmazuqj.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2wppwdfpe.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2bakiywmf.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2donafusf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewsykhhr.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2xbjtpqoq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2owklfelj.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2ckzxwijb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2wnjxysdd.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2ehqyfuss.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2ktavidkd.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2pejdcenr.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2huifssfv.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2tuslsect.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2xigwktij.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2qczsxqhm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2hehzhwam.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2dvimrkzn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2lgbjasmi.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2pzgueqmr.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2qenszqov.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2ibizmrei.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2axognemc.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2biwnfrzg.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2qwxenuqb.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2xotlrljy.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2fonasyrd.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2vloopbtk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2pxamnwyz.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qmqohmle.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2pbujhygx.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2jxgmujzl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2nabxsqou.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2mmzcmjgq.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2typqlrmb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2mutmjfaz.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2tpsyemhe.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2gtolzdkx.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2rpuhqfrn.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2sarrufyh.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2zlizqrdu.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2vqfiiivo.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2dcpuobcr.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2yvwnroti.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2jajjvril.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2nprkjmom.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2tvdsgswa.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fnlpvtsa.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2oavimyck.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2xoinryei.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2zirafoid.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2dtebwcto.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2vhhuxucc.html


<!-- 参考信息 -->