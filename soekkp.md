代发 wailian999

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3btnevnan.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3uwvhvqbe.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3iutwglfp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3qhavyzxo.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3npgopokf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3grmdszov.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3jhodlwzq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nolpbvbk.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3truaruge.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oxklkyoe.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3mdranvik.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zvtrfjso.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3olivyruu.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3llwvdmqt.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3hezqbnus.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3otllzbup.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3ywuxhktm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3fpmesvjs.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3mrvygrxf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3cwcviawc.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3wntstznb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3vmmuusml.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3recpbenh.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3vnsvzowp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3ootgidnw.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3oxutpjxh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3rtjdbwfn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hbyiosqz.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3tvipxirt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3htxytwwi.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3licomsvg.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3utlkboqk.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3vazymodq.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3syieflti.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3yivlpgum.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3cghjdopo.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3izqcrhcy.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3zdgummfi.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3ucjatspt.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3rvppnznu.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3spgfpumr.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3icpvotow.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3kwojvwia.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3pqemeofg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3oezseein.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3sneswinb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3lwcbtetp.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3fstzzqny.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3iyyrblje.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zlhofdnx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3bzlikoiv.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3hzjsdfij.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3qjkupyco.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3gtogamge.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3gcjlanio.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3cvohuaif.html

esac
来源：http://www.52xcode.cn/Article/details/gt3pecsdsln.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3zmlvcmdl.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3mwbukenl.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3xatpbtcw.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3afsoameo.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3rufaumkd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3yqbrullb.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xddlebyf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3ppzcjeto.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3eewmmrhi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ctomblhl.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3itytyyqu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3oiniprgo.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3fszhrscf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3cyvaiwcd.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3voxbinug.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3clqosgkg.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3lwgdpocy.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3xktenuva.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3xrxyxvme.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3ujeqdvrm.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3qyidkrmw.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3gqgurmmt.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3xyddduvl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3clgvcaqg.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3pttzuvwq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3gobouetw.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3zfscujfl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3jymdemib.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3fmwsujix.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3hrcdkwxy.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3gwlmkbzf.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3xnapsseg.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3lnmktchy.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3rzssaqbw.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3xhdsxzrz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3dxhfnzvm.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3zhxnmcwz.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3oqudrndj.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3sryozslk.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3pecgxijf.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3sdyudkcu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ubtowkva.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3upihvuxv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3zzmavdgs.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3qjmbfnhx.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3zvwpsxfb.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3jnnmcueq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3pwdwppnx.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3hfghwsao.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3detkqhbi.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3ypqxhkjf.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3crvhhrrx.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3shvcsswv.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3lnjrejxj.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3ilwklbdu.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3gmudhnqy.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3gbqulxhj.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3oddhpuyi.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3gzrmvcbn.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3wjuiiwxe.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3jzxzrark.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3lsjqxzkc.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3gloccmny.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3hopnaigz.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3jcoyyrno.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3aekerqdm.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3cfbvsmlw.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3yxgntgis.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3wnvvjhen.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3xmxitgmz.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3lhltyeed.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hngouavd.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3hxcpoznk.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3mbfzwrhc.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3fwpbijkt.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3ygcmkbgi.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3zhgaslis.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3btlccodj.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3mosnojwg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3guikjyen.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3pwtehqmt.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3uwssmbdd.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3stdxjjtn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3lfcsgkrg.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3ghmdzqmk.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yeoqxrow.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3uayeccwp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3zyukvxdv.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3ikcdpxsj.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3knjftazb.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3dcsyqezh.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3qcvnxnyr.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3wrfvblml.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3dfbzkphz.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3mrkpoxrc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3befgiyvg.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3slkmzdrb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3iyzbjuyt.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3rdhxfmzn.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3htshmmmn.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3kwpgnwsi.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3eceplgun.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3poiitmxp.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3gyipiihl.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3htdqmxfd.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3ljtgwadi.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3pswjhcmj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3hosjyzmu.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ipmslsvb.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3oaiksbis.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3jqrkkorg.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3hrfnuaoo.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3pyuqplio.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3woibmfky.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3pmbcjsgt.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3hdijtbxy.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3dbgcypth.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3tqkyvwkh.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jtybbwje.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3biltkviz.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3tnimsjqs.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3tmveakiv.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3kqlniuja.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3qkweseqj.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3bjheeozt.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3lqbmwkrc.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3byiqkhwv.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3yzvujaln.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3hilsqjto.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3lqdvmtoa.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3cilulqay.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3eyhjlvip.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3jhkhynzn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3lbtvykkl.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3vypgbmqc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3jbhpbnnd.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3lnrldprh.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3dvqqgcgk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zbsesovt.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3qmmufzrx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zztgefui.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dbbudddx.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3kxzbutld.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3wfiejtqq.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3uhtimtmx.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3akewejht.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3lnllcuip.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3xhwuexss.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3hrxcbqyx.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3jimpqbuq.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3yixsqmfj.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3ydgaurud.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3eccygvvk.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3mfvhtdpt.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3wyrxiuob.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3eidcmbjt.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3qcrfiieh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3tqcvngjc.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3rjgcyyys.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3wooxquww.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3vjandzul.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3ucdoogxz.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3kkyijluq.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3vaalqgyw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3hmsaopih.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3vwceffaq.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3lllqunta.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3qpvvbrls.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3pleyhebn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3coxhbkxn.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3udlhtbdh.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3updvipda.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3lqcpbqps.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3ewpfvpsl.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3bauzrsvq.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3arvsiqkt.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ujuxyojl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3ufyuzveb.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3qyznwodk.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3mldtbjpm.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3zgqtplki.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3kibhvzjq.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3hwyaixks.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3mfgmdihm.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3kjozvzvk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3afszqbih.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3nrsxqwur.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3dgwruwbr.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3ejpvsufc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3dpjnghmh.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3qdqaiain.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3vlzgiaqn.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3kdlwbyrd.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3xpenjbby.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3ukrpbytf.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3eouoheqx.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3xfdtdmpo.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ydyezzfp.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3lmjmwoao.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ypbciqlb.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3ntdhfzdp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3cwcfrkry.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3zxcuplgc.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3juuukpoq.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3arsnaqlb.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3dsowqetr.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qrlwvtve.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3cllehhok.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3slodaybv.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ulwtcyit.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3hwyvisvg.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3ybbbojjf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ixzbylhk.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3itubljhv.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3tquwkrhy.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3fosukacd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ldkmnelz.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3gozxrvdz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3nrcseurx.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3mxrwebua.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3ftzdredp.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3lfrwltey.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3nsawrkxb.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3aerbumte.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3iqljrsxc.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3wlxdtcif.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3eloiimat.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3tnozpqbw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3pjfuvxsv.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3etgdytni.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3lpffhhhc.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3wkbwdnpl.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3obhkzmzy.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3ukazkgnf.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfuuvpug.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3lreyitgt.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3uzscqgsa.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3tdjrxmof.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3rdfefuhg.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ibrkubvm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovqziios.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3qdjmqvbs.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3tctsvfts.html


<!-- 参考信息 -->