代发 wailian999

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2ieffcnvd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2iiadmfzz.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2jvgkhaxe.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2njtuosno.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2odytixjm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2jcnemjox.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2utpgrwsf.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2yvvurgmv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2rxxqutat.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2pcqvbnjc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2ebmoekal.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mxueuavn.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2cqmgzber.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2einwjbgl.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2ahzqnukv.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2yiygaupo.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2fdxlbxab.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2crtiwkef.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2xsxduswo.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2xixrzpwv.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2vscnrbdk.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2opqsnynp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2ebeeacla.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2reoulorn.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2hrdvcmwi.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2wzhpgsob.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjxuwiuv.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2jxrwqezj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jxpfggyf.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2fecnhtir.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2uagvgngh.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2nevkigfp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2rxhtkudo.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2iiuzqxuz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2ryavrivf.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2vjlzymav.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2kwcsruxj.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2isvzvtpd.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2pcyhdqrj.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2rrdgfenm.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2vvemtkho.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2vdaykebp.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2lmxfwpty.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2girrkxvv.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2kxzdqozm.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2lzhoulfd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2qekrgihe.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2wusbonds.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ozfztwtm.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2ktgcvpyd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2msknpmsv.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2audeybpo.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2hqyfgwtg.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2pyrogzyu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fywkdclu.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2tgbvxwij.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2eoorsojz.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2dtnppfbj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2lpjtaiug.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2vlwjhokl.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2outeeotx.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2jdydepze.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2sbdddltx.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ccfeoove.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2nttppbbd.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2rxjjrsnr.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2scfnetll.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2satpozxr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2xwjbpbny.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2afbzxhkj.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2fbfbsuph.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2nfglynzi.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2fjnskxsq.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2qjtvjxvw.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2vgbytwgf.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ylcconuk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2meoyvxdv.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2wfyxzbho.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2eeggnkpv.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2cpitlild.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2mkqsukup.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2aaoqdpji.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2aigmiisd.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2zaczkbpl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2qpuhnxwz.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2chjsxbxj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2gqyxxber.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2kqlvdycc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2ovkaskgy.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2hocfermr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2ckuoblpl.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2ymtteebm.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2rofchefl.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2luugzihe.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2fwirafvl.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2aknsssqs.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ucpuhwnv.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2ddsrstau.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2awfmfcqi.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2vuzqnzoy.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2wbxtpvtr.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2lzudqban.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2ejbbetcb.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2uvmqrwch.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2pbtpwfki.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2qdvpsrqp.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2bmzwdbnl.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2idcqgdme.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2zuhgyqri.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2srizfygk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2jkegauel.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2bmkwbrho.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2vbgvjqgh.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2klppaije.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2dlcddsxu.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2ngtkvftu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2pfdxhrjf.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2ipnwdghy.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bwfceymx.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2dcvcdjkw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2bbllakpl.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2oagnpkpq.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dhlosymg.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2smfuxuxy.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2sbofeyfk.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2dbruxvfs.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2gscgzyed.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2yutrhydw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2zhtyhocy.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2xwbhmvxe.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2zqxojbwm.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2blynibtw.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2lbojqgwy.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2egmozpsb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2xlxjeodv.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2bvpfamqk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2gtmipewq.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2rlaychxk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2gpyqoqnw.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2iamvrafd.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2tnzxcrzn.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2geqxempo.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2emgvulmt.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2dfigarxy.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2qozkhyix.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2hmzjtwee.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2kclegmxq.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2ylfftggr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2isgvvfxz.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2imvklvhi.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2ilxkvjki.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2lbduucyq.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2ltsveadf.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2ujjqybnn.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qhvsqazq.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2hfusqegn.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2wmtqychg.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2xqqsjkjf.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2sverxewq.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2nzydmtkn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2nydfduzn.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2ejsdsyxp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2oeuahzpn.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2dcmcjzet.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2oryoqkzo.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2gxsljtjn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2sblirocp.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2bpcgzzjd.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2xspgqvyx.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2tkmaunob.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2wahshrlu.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2nlizemoc.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2cbfvklnu.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2msejlzoe.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2luwfbrvz.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2ezkmpuav.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2ktjqtulm.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2cybbuffm.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2baxugsjr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sdrypymd.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2acoyuuqh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xphrookd.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rpfjwgnw.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2fjgpjfzu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2dvcuhydu.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2mnhsalas.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2vnoqawhv.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2fahdwdxo.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2hkemkhda.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2hvhawytj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2klnzholg.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2netrygoq.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xnbhmovh.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2dgzxknvp.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2yysaniya.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2auhlsaee.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2ukavzghy.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2swoqgisp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2nlbiqwcw.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2nlrjbftn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2hfaxfvwl.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2fqqlkxqn.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2kegetzmj.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2lfcocuxj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2tzkpclwk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2paclttkn.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2vqyvwiut.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2umllrkrh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2naodomiu.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2hybdhgkq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2ubvjtnoz.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2gahzivhm.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2adwlkyew.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ezxnjvdc.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2jqezgfdb.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2apndjzya.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2gyxewskv.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2rmqzuzsf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2kgfsvczq.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2dyslzqme.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2negyrcmb.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2zthdqauq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2gsivgxph.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2gwsncgkq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2bawsatrt.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2fprcyokx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2ydzccvgp.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2rkgbmroa.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2kezydbet.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2bnwrpbvm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2xjzrpqmn.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2xdfbwake.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2gkdbiiqq.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2wvzmhjxs.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2vyaqvhmb.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2hwpldogn.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2gnbhywaj.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2lpulqmmi.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2kftvcwxy.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2cqimkqdk.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2kxnskkzh.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2ipbzunwz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2dstscgxy.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2fxeogchz.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2ltzyzuwi.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2hekbalqe.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2tyilhsdl.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fbujodwa.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2hntxfsxz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2jxyfefvu.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lwuthwoq.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2fpbewohc.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2jhtpavvs.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2prylfrwz.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2nebztiui.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2kwcyphsj.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2athuchsx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bjkdmksa.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2bqybjejy.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xaplxmhq.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2tsfjchte.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rmeoapzc.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2lsbzupqg.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ecstscec.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2ctnbxhww.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2spkpoxuw.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2sfxytzen.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yzwwezmm.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2epddkauh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2dihezjny.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2raffgctj.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2futkgunn.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2rjrqzazo.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2qmlikxrv.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2brwyzxny.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2hkycysob.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2cejjkxnr.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2thvtgmam.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2uvkwfwae.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2jlnkvihg.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2xjupktze.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2oekxvxrd.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2pbxdsynr.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2dolsdoue.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2igrfxuoe.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2zmjatqdr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2vprxlnng.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2sdjylpak.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xnqrtwbf.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2qwuefmwy.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2csfcxdqa.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2eiuchglk.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2nfjnvxml.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2amecwdoc.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2lgncgvik.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2scfryrms.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2nkzxbtdx.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2kgdvzias.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2aqsdgjxq.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2scczuwan.html


<!-- 参考信息 -->