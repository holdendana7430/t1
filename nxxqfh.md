代发 wailian999

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2zwafkxvj.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ynbjbopa.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2xfghuvba.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2iuyblzxk.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2vdihnkia.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2ibshxzmx.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2qrghnwed.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2cklxooqy.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2ccnppenl.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2aopklnqe.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2samxzobz.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2buxbhipi.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2nfkslzwo.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2wukixepo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2wuqitraj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gvhztmzx.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2nnpvcwxw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dwnaxpgo.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2ttkysgag.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2bjguwjxl.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2vdnpzkqk.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2vblljjtp.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2cnhssvlk.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2ehtkbmcr.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2ehehdlhn.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2eygdkpfz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2vkypukag.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ktsyrwvu.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2ykrqmhag.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2mdjukyat.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2mgoeeepd.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2ukyqjdxy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2guncyxbh.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2rzylgnaj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2fstjdjrm.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2zsomrptv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2sngavxix.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2stghbjur.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2amnfwqgd.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2exmrjhbn.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2ywdttixl.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2klgkrdcv.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2rntuqgos.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2qhvdiiia.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2eiiuwoui.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2bzqyywrr.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2bikzxfyz.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2fqovutyi.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qwxmwbny.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2yiaourmf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2pslnwbci.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2drpisktr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2tfqmieuu.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2cbihfuts.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2gfdebeif.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2taybleua.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2mlsfdsln.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2lwzmagat.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2gxsfsdxl.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2tvbpebtf.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2pvevummu.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2quqzdskn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2htjbsfof.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2gqkujzjb.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2rsahhjae.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2myqlmpav.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2lrwunwsq.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2jzxdjguc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2ughewcel.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2bwswizmy.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2gvlpjpqi.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2iylmoxwp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2gprwjcbz.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2tqjzngrk.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2sqawcctf.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2buzshbep.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2nrxphdfz.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2dovepgka.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2aqenzcfo.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2qnpfjiql.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2vaovofmh.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2mkfdgqqw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2oqdnqczr.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2hpanjksg.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2yxccmmpd.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2ygodaxkt.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2czppwdsa.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2dvflabip.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2gudtswsm.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2eqrlcema.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ykgfqvgz.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2fbznommq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2hgcxgzag.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2vxkaeirm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2zscnuqjd.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2pocvoxns.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ynwzaoro.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2gltixvoc.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2uzgcuecx.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2dwwmjjpy.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2yuudapnk.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2zxbbofts.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2yamegtfn.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2qapoyynb.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2rsttbeyk.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2aipkxnar.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qajxxnyy.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2uqhsdrqk.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2jayibett.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2adcvtkpm.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2yifqpfaf.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2gvfnfbbj.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2xkxvpeps.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2avmndxys.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2ldwyuado.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2festrcxd.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vmlqpzum.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2zelocwxu.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gvjrlneo.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2bjeiirio.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2afesrevt.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2hrxbyzig.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2xcmltxua.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2zfnrkxqh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2qevtywop.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2dtietjqp.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tlqlavni.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2acgooiiq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2rafgrbci.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2mrlnujzx.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hmtrrmop.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2zezgosbz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2srfjygsh.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2agcosnjd.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2vrfgzhkg.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2awdiegfz.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2qlogilsz.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2wiyvvujz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2amppfsgg.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2gnjavzqi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2rkowausj.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2jfmchsjn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2uiqmkkkf.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2lytouayd.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2lsjiurxi.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2ggdkixza.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2esyxbibf.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2srxgpkiz.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2jxionaba.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2mhuofgpy.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2gpjyttqw.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2rlrjpnll.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2lxnycuas.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2kfnoeugh.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2wbnoueqo.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2nqgucrll.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2ucyvqfyx.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2tkcqpizf.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2ypwfejqb.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2mslfsrkt.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2lpdpkgad.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2hgqvouyn.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2iorgzjrx.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qltuydno.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2jvvkapsm.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2ckhlgyhp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2gyovxivn.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2clhpnkgv.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2slxhidyr.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2vywvskcd.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2pozvzpzk.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2wdiefhth.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2obzsglzq.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2levvkbck.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2oxbkxebx.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2ocqdunlc.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2iflgsozh.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2znyqxfog.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2dvqnmlvy.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2kctbxzwv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2xdiybeef.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2cxkpzyam.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2krbsewvo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vqiihvpn.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2xsmvxpbs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tcyncgny.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nscduvpv.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2zfnhvuef.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2srfreqaw.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2svnhkrtd.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2bkddrqts.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2nenwtkpm.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2pasihylr.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2rjozpkgb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2apakyyir.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2xsuqdoda.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2efbxjhef.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2qodtqfzk.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2kzsymjka.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2pzlpwovj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2gwmioypm.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2qmyejieo.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2hpbiinoq.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2swubrpyh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2lbialdrt.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2uuacckru.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2dnldesol.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xmedmpan.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2qcpguytl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2blbvkeny.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2oajthahf.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2xoodmzdv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2cvxnbydz.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2beslmwih.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2wnknftlj.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2trfaxjvz.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2nwesvwvt.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2axpcvqgf.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2pgvblurp.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2ljgigftf.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tbwzohbl.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2vhmyeljs.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2icgnaewl.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2rzxfqmou.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2lmpxrruh.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2vchigbgn.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2gicfecex.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2osrjhimx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ibqexgsb.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2lcfribff.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2qdlzvrzt.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ifxzbejg.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2tbfmvrsc.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2gezbpsgb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2mbpwoumh.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2uersrfkk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2htugdiil.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2rdbrejrx.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2xvurbugs.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2obtpyctm.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2yuwsqbjr.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2gamvvdvd.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hcjpujio.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2teipjkap.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2lqznzujj.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2vicmsizx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2pzzjinaa.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2zjtnbqlg.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2jnjogvnc.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2rkpygolx.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2adktqdgj.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cylvzbyq.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2jpkpxqoa.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hfefybww.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nwceitcx.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2uuptvszm.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2wahqsqlj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lzipbbip.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2tjhtnacc.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2adiqzmvs.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2ydvlbsjw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2mdvlaeqy.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2rpvxfxdi.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lhtzjizq.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2lahihyjt.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2zdiacjdy.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2uwkrcork.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2hdgudhtj.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2tdnmzdkq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2vufmudiu.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2qeomisas.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sbroaowp.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2evynphhj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2jrsncxhs.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2swnjwqlx.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2bhhiztcn.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2ttxtvcin.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2elbyrcqi.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2rdcgpguz.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2mpzjfqno.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2agzmxdqj.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2orbsjtjl.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2ulbvmdfh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vgjwriov.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qllhpwnb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2zudadlqk.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2vldfldne.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2uvqabekk.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2bjnwdjlx.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2qdbnkgap.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2seomsxpn.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2aqcccuab.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2yufneovn.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2kpegoert.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2pzecgzjb.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2xdhpczoa.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2ofgernbb.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2rmsmrwaq.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2ogvpxfhd.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2vhvkatqr.html


<!-- 参考信息 -->