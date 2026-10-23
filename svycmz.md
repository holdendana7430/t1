代发 wailian999

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3xymuocnc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jmhxrzzj.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3hkiqwuoe.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cflfmcko.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3kzkzolgz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cpdacmcp.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3cqhmxkkj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jptsjbfp.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3hyxkcyvc.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3usmgwyxn.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3rhpasodl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3eiwknczt.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3ofxsqfdk.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3nurhhhbj.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3syjyacwu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3ounwrzwd.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3ppxlltfw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3ouiumxaa.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jonrinxt.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3fbsqjqad.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3eyxojdhc.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3cjuthqhh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3ptbewwvl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yplmannv.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3lnhamtgv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3elnymtpt.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3yxpxhrge.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3zmxyyffq.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3nbygvvod.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3nlznfwns.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3hehhsbdm.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3xdytvbhy.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3ftckbvje.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3qxbtwixj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3hzaaxdzc.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3jpnuplqa.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3szyazlzs.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ibltkcrj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ejkdqqma.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3yhczffjw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3gkaptxax.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3lizvgutb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3hgeosflg.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3foxpibyw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3wignafyh.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nbipmcoi.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3isakiizh.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3flvsetqg.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3viusmwye.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3nmrdsefs.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3gfqffacj.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3rdtvlbba.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3vlbfgjmn.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3wwajzind.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3gdbzyqyi.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3xqtmfxwj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3jyzkxskg.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3wgvqarvw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3aaksuwzk.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3lgwtbjuj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wprcndkc.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3kzxurzhq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3yyuxstbo.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3puuxlygj.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3sryybzul.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3likxppvd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3ctjhdxpi.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3anilxtvp.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3pfzixupg.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3xvhxiybq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3xdadhzbd.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3kzhhwqbs.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3umwboopc.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3dvtafonf.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3bgwelbmp.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3frjocoww.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3uxexaivp.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3pupjlavg.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3mxpxouwz.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3ztgwudvb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3dnszcdqi.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3fmvbbxqo.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3rpkdfydg.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3cdtejvgr.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3uxsksxes.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3xiifuvxw.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3chprueth.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3zpmvbytn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3amqrndni.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3niofgnpj.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3dtvrnsld.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3gvscqnvl.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3jrgxkoya.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3bfydkepx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmsdjhbk.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3cmlvgtjz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3zezkszag.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3ltlinaho.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3sezvfyht.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3jvydkfqo.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3fvxilihh.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3jixucyno.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3mpzogqhi.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3wiouewrg.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3eehsebhi.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3wkuvdema.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3gmncrtgi.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3ltwgoufq.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3kbeepjdm.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3scxzraqv.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3llnbobnu.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3dryyltao.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3nzsmzqio.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3ikmsxdan.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3hvnjcdsi.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3gekpfvyw.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3fhnltvso.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3fcfhqrad.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3ogznpvtl.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3cdlguful.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3ggirlrwp.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3qlbpjate.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3twlcbokc.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3iwsmnfww.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3bqyorbag.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3tklbhvis.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yrzwesjg.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3hwprprqs.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3uaoguhxo.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3uobnfzvd.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3pbjwuhov.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3glgtntvw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3vhjogxrl.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3sbndncji.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hcphjxpf.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3uzknqdtx.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3tpuztbcx.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3rsxkmyzp.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cmmcdjxf.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3ojldnrne.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3mipjpzlu.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3fdjphecj.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3tqvwvecv.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3vajneqra.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3dsrlzpyj.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3mlbukenq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3uuwqhhit.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3wmkkpttc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3varxwzli.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3fwvoiciv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3cjukwspm.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3kbddeamy.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3vqcftinn.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3zjdiywmh.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3hszohyex.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3ihxmjmot.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3rwvccyny.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3pesvxsme.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3pssnveyo.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3ygaigstg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3lpirehqq.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3fjuaunmn.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3zgujpaqg.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3jsoafqhs.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3maocoyxt.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3xoomieve.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gzaugish.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3rywynlrd.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3ntquldie.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3qyryavuo.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3gfbsfhst.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ykqeikuk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3foeiiwtq.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3vikpjnku.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3gssifmqu.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3xcitpwmh.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3pvedyjyt.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3qtgkfpqx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3isojtbzh.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3gukobpws.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3qygwkmui.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3ewgcfqgr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3uegqnahu.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3efcroaie.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3pjjhhfwn.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3hcgqmebl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3orvtzemu.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3dmmvkndk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3zktcqsuh.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3ntgeessm.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3eaqqvhzf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hmopneig.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3kzkhvzwv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3miapffaw.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wclvapzn.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3bzhrdlxw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3ljwwdcgv.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3xkddnsni.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3oichetsj.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3vckftehr.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3apaavojr.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3snnnzrew.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3dnkrfuwi.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3dubddawl.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3ryuwtiuk.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3vhjuhcyh.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3lmqjqudb.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3raozqfuz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3vlsocewb.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3znkuycfg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3dqtdzucd.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3efheuknj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3vmcqhyuh.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3wwizcuoa.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3naghogfl.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3inqaznvx.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3izhvqwhm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3gokyaiar.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ogvqdeba.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ffnsmbeo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3mdcuhsdb.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3kwswdmnr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3ekkmbrgp.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3jcmgxufh.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3dhowjqus.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3nyjtjrxj.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3fygfrwrm.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3nkuuhjba.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3yedyuyvj.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gtauktov.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3xsevdksq.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3rvtnjyrw.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3acclwlqs.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3fjchydgu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3rybonxhv.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3nnrmnfhj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3monkbqpu.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3qiephold.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3qecofcln.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3yzgcngkc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3ajoegyoi.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3vziadcdm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3kaqwlsrv.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3axlwbwor.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3digaoqil.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3rqxrxsxw.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3pwaizvvv.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3jyshaphv.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3oopccxlg.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3yjepxhjs.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3aahmbhkb.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3vzlzcnqj.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3getqbibq.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3ascimkpl.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3axjjscfk.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3ulkhqvyr.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3lozrguxm.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3djqotmgx.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3bdwvrxod.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3oiwslcio.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3awadqnan.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oqwlhneu.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tuybnszb.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3xeznesvs.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3kxebhvos.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3cawykdln.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3yobbdqvg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3ryqqopzd.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3cqdszqrd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3pawarnua.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3mqlgegnd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3agenkhvo.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3hfdeixiq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3bwcdhrqr.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3guyeabzd.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3wtjyglrs.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3oakhmckl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3tlzgtvjg.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3pfhsonad.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3iannvibi.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3jnadoduq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3jalqjsfk.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3qcexdvyz.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3tgkczbdb.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3hyzghmsy.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3rgnolkdy.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3pjsptbnb.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3lbojpnca.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3kbcndpnq.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3nksfsmlh.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3vngtzrey.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vlxnajvo.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3vjduvhqd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3ttqyoupz.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3avukwpdv.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3xnplrrlo.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3mbpwnaca.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3jikwgywv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3azqxhrbp.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3eqsaxbei.html


<!-- 参考信息 -->