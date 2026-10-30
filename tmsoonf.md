代发 wailian999

[Q78] 当前时间
来源：http://read.share.fehbvm.com/Article/details/gymsfpmnf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fehbvm.com/Article/details/gvwwmplmn.sHtML

[Q79] 字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/grxorfazd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.zdbjq.cn/Article/details/gjnsdxvaz.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fehbvm.com/Article/details/gwupczkul.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fehbvm.com/Article/details/grfurrugl.sHtML

[Q81] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gfsxkdztt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fehbvm.com/Article/details/gcltqxvie.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fehbvm.com/Article/details/grrkkvzfu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gefnloilr.sHtML

[Q83] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/guktrwppi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gdgwajlic.sHtML

[Q84] 去除首尾空格
来源：http://3g.zdbjq.cn/Article/details/gqznzyqws.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gnfklfgij.sHtML

[Q85] 数值取整
来源：http://www.m.share.hesvh.cn/Article/details/gedptehio.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.zdbjq.cn/Article/details/gxgqjsppb.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/gthqcprlu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.hesvh.cn/Article/details/gxbuxzdra.sHtML

[Q87] JSON 字段做条件
来源：http://blog.hesvh.cn/Article/details/guecpkomk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.hesvh.cn/Article/details/gesjynhqw.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.zdbjq.cn/Article/details/givmxfoae.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.hesvh.cn/Article/details/gepvsrinx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.zdbjq.cn/Article/details/gmbdztgpd.sHtML

[Q89] 判断表是否存在
来源：http://wap.zdbjq.cn/Article/details/gqfubntvz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.zdbjq.cn/Article/details/gxnorbqff.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/gpnkqsqzz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.zdbjq.cn/Article/details/gkgvwsntt.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ggbyghotk.sHtML

R. Bash 专题
来源：http://baike.hesvh.cn/Article/details/ggguarech.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grqmjkwhb.sHtML

[R01] shebang 与严格模式
来源：http://read.share.zdbjq.cn/Article/details/gkhxglumj.sHtML

#!/usr/bin/env bash
来源：http://www.share.zdbjq.cn/Article/details/gxauvkdlx.sHtML

set -euo pipefail
来源：http://www.m.share.hesvh.cn/Article/details/gueiqmfhc.sHtML

[R02] 变量赋值与使用
来源：http://blog.fehbvm.com/Article/details/gyqxbkskl.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.hesvh.cn/Article/details/gbiuwtaqa.sHtML

[R03] 只读变量
来源：http://3g.zdbjq.cn/Article/details/gwjmhraqn.sHtML

readonly PI=3.14
来源：http://baike.hesvh.cn/Article/details/guvnxmoma.sHtML

[R04] 位置参数
来源：http://blog.zdbjq.cn/Article/details/gfysxpvul.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.zdbjq.cn/Article/details/gdegpumjb.sHtML

[R05] 参数默认值
来源：http://baike.hesvh.cn/Article/details/gfpifeaik.sHtML

name="${1:-default}"
来源：http://www.blog.zdbjq.cn/Article/details/goohcgqxn.sHtML

[R06] 判断命令是否存在
来源：http://3g.hesvh.cn/Article/details/guakoqtki.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gpeydkiqy.sHtML

[R07] if 判断文件
来源：http://read.share.zdbjq.cn/Article/details/gbnqkngfk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gimxnzjax.sHtML

[R08] 数值比较
来源：http://www.share.fehbvm.com/Article/details/gqneotkwc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.zdbjq.cn/Article/details/gmifexhbf.sHtML

[R09] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gacfuzrxu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.hesvh.cn/Article/details/gppsibdzs.sHtML

[R10] 正则匹配
来源：http://mobile.fehbvm.com/Article/details/gvtgyibye.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fehbvm.com/Article/details/gtjhmqepf.sHtML

[R11] case 多分支
来源：http://www.share.hesvh.cn/Article/details/gicclgios.sHtML

case "$1" in
来源：http://blog.zdbjq.cn/Article/details/gcyjpamrp.sHtML

start) echo "启动" ;;
来源：http://3g.fehbvm.com/Article/details/gxlzrcsif.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gxayiitgv.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.hesvh.cn/Article/details/gqyxmurgk.sHtML

esac
来源：http://3g.fehbvm.com/Article/details/gtljdzgdr.sHtML

[R12] for 遍历文件
来源：http://mobile.fehbvm.com/Article/details/gwjgqlhbg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.zdbjq.cn/Article/details/gvfcpdklz.sHtML

[R13] for 计数循环
来源：http://www.blog.hesvh.cn/Article/details/gbghlovvw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gmwlipppr.sHtML

[R14] C 风格 for
来源：http://www.share.fehbvm.com/Article/details/guimmucoq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gxzskyrle.sHtML

[R15] while 逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gsmvpqobc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.hesvh.cn/Article/details/gvixvnodb.sHtML

[R16] until 等待条件
来源：http://mobile.fehbvm.com/Article/details/gkkhrdrgv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/griljgtyy.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/gyalxcaiy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.hesvh.cn/Article/details/ggpsvhlgo.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/gkpgspnid.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/glgevxmfh.sHtML

[R19] 数组长度
来源：http://blog.hesvh.cn/Article/details/gcjizmceq.sHtML

echo "${#arr[@]}"
来源：http://mobile.hesvh.cn/Article/details/gczuivfbh.sHtML

[R20] 关联数组（字典）
来源：http://www.share.zdbjq.cn/Article/details/gdwbxqeet.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fehbvm.com/Article/details/gwomhuwif.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/gnwqeseiw.sHtML

echo "${#s}"
来源：http://blog.hesvh.cn/Article/details/gglmdleae.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/goruwrorm.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fehbvm.com/Article/details/gwzldshml.sHtML

[R23] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gaaolczth.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fehbvm.com/Article/details/gztbscrak.sHtML

[R24] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gltdfycfh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.zdbjq.cn/Article/details/glwldxown.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fehbvm.com/Article/details/gtjiorpij.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.zdbjq.cn/Article/details/gwyxlujfl.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/grtjjwyvm.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.zdbjq.cn/Article/details/gmdtanyre.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/gzggicbmz.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fehbvm.com/Article/details/ggdmjhegm.sHtML

[R28] 浮点运算
来源：http://read.share.zdbjq.cn/Article/details/gnusorrsd.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.zdbjq.cn/Article/details/gwdohfxlz.sHtML

[R29] 定义函数
来源：http://mobile.hesvh.cn/Article/details/gruyheuwc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.zdbjq.cn/Article/details/gaxrtpife.sHtML

[R30] 函数返回状态码
来源：http://baike.fehbvm.com/Article/details/grasnscmx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.zdbjq.cn/Article/details/gdfdsprqt.sHtML

[R31] 局部变量
来源：http://3g.hesvh.cn/Article/details/gkxunnahz.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fehbvm.com/Article/details/gxmeqoprh.sHtML

[R32] 参数个数校验
来源：http://www.blog.fehbvm.com/Article/details/gpfyllqcj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gncpvtfdh.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/ggfqcnuas.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.zdbjq.cn/Article/details/grouytkla.sHtML

[R34] 退出时清理
来源：http://mobile.zdbjq.cn/Article/details/gjxuwboxs.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gejdbznrn.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/gibvxhfts.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/gqozxnriq.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/gilczqikt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.hesvh.cn/Article/details/giavzezck.sHtML

[R37] 把输出赋给变量
来源：http://baike.hesvh.cn/Article/details/gagffixiu.sHtML

files=$(ls -1)
来源：http://blog.hesvh.cn/Article/details/ghrvlintn.sHtML

[R38] 管道串联
来源：http://read.share.fehbvm.com/Article/details/gibhwgnam.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.hesvh.cn/Article/details/gdwqlufrr.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.zdbjq.cn/Article/details/ghhgbcykf.sHtML

cmd > out.log 2>&1
来源：http://mobile.hesvh.cn/Article/details/gaospixvl.sHtML

[R40] 追加写日志
来源：http://baike.zdbjq.cn/Article/details/groluddhs.sHtML

echo "log" >> out.log
来源：http://read.share.zdbjq.cn/Article/details/gfjlejsqw.sHtML

[R41] 丢弃输出
来源：http://m.share.fehbvm.com/Article/details/gwavbomeb.sHtML

cmd >/dev/null 2>&1
来源：http://baike.hesvh.cn/Article/details/gfyybxhib.sHtML

[R42] 输入重定向
来源：http://read.share.fehbvm.com/Article/details/gjjxwqdls.sHtML

wc -l < a.txt
来源：http://wap.zdbjq.cn/Article/details/geaeieptc.sHtML

[R43] 按名字查找文件
来源：http://m.share.fehbvm.com/Article/details/gildrmknq.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fehbvm.com/Article/details/gitxydery.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.hesvh.cn/Article/details/gtxuilnjv.sHtML

find . -mtime -7 -type f
来源：http://m.share.hesvh.cn/Article/details/gklaehrba.sHtML

[R45] 批量删除
来源：http://3g.fehbvm.com/Article/details/gijbfwxci.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.zdbjq.cn/Article/details/gdwiprguq.sHtML

[R46] 递归替换文件内容
来源：http://wap.zdbjq.cn/Article/details/gjhzazchc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/gylmgnojt.sHtML

[R47] sed 单行替换
来源：http://www.blog.fehbvm.com/Article/details/golrgrwgn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gkeyfymep.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/gjllnrwze.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.hesvh.cn/Article/details/gubwjpcxh.sHtML

[R49] awk 带条件
来源：http://www.blog.zdbjq.cn/Article/details/gocoxndls.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.hesvh.cn/Article/details/gehondrsf.sHtML

[R50] awk 求和
来源：http://read.share.zdbjq.cn/Article/details/gbalpcxlc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.hesvh.cn/Article/details/gzwlvishd.sHtML

[R51] 排序去重取前几
来源：http://read.share.fehbvm.com/Article/details/gjilhkemv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/gncbsexeq.sHtML

[R52] 统计行数
来源：http://m.share.fehbvm.com/Article/details/gsaoxmfbj.sHtML

wc -l a.txt
来源：http://3g.zdbjq.cn/Article/details/gkojvfadt.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.zdbjq.cn/Article/details/gmmyvmsfe.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.hesvh.cn/Article/details/gwvvghwrk.sHtML

[R54] 比较两个文件
来源：http://blog.zdbjq.cn/Article/details/gugnryprg.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/gddokhdbd.sHtML

[R55] 压缩与解压
来源：http://3g.fehbvm.com/Article/details/ghxpuhxsh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/gvvghdbsc.sHtML

[R56] 远程拷贝
来源：http://mobile.zdbjq.cn/Article/details/gewbzlljj.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/gghweewti.sHtML

[R57] 远程执行命令
来源：http://baike.zdbjq.cn/Article/details/gpxbfpdpv.sHtML

ssh user@host 'uptime'
来源：http://mobile.hesvh.cn/Article/details/gdclgqozu.sHtML

[R58] 下载文件
来源：http://read.share.zdbjq.cn/Article/details/guwjgfdgo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.zdbjq.cn/Article/details/gjjcjjfst.sHtML

[R59] 发 POST JSON
来源：http://wap.hesvh.cn/Article/details/gcnjtadoa.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.zdbjq.cn/Article/details/gjpjmqwqg.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gqtybgiqo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.zdbjq.cn/Article/details/gpstbxkum.sHtML

[R61] 磁盘占用
来源：http://read.share.fehbvm.com/Article/details/gqnafbsrl.sHtML

df -h;  du -sh *
来源：http://www.blog.zdbjq.cn/Article/details/gwdgyfejp.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/gwkiicacv.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fehbvm.com/Article/details/grxbzmdev.sHtML

[R63] 内存与进程
来源：http://read.share.zdbjq.cn/Article/details/gphoavrfe.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fehbvm.com/Article/details/grbjdjilv.sHtML

[R64] 结束进程
来源：http://blog.fehbvm.com/Article/details/gqueswufc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fehbvm.com/Article/details/gosabmvcb.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/ggrhmyhlg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fehbvm.com/Article/details/gsrbrmslf.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/gjtagdxcx.sHtML

crontab -e;  crontab -l
来源：http://read.share.zdbjq.cn/Article/details/gcelxisme.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/gmhenaueq.sHtML

openssl rand -hex 16
来源：http://m.share.zdbjq.cn/Article/details/gympwglhb.sHtML

[R68] 计算文件校验值
来源：http://baike.hesvh.cn/Article/details/gjyiiqcso.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/gauferqcw.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/gdqrugoho.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.zdbjq.cn/Article/details/gviwxqkue.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/ggkskzxga.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fehbvm.com/Article/details/gtrwuhyey.sHtML

[R71] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gcidorifb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/gbobivjos.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/gpmbwiqes.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/ghgxfyfrg.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/gehdbilzb.sHtML

split -l 1000 big.log part_
来源：http://m.share.zdbjq.cn/Article/details/gusjknmif.sHtML

[R74] 批量重命名
来源：http://blog.hesvh.cn/Article/details/gcsfmkake.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fehbvm.com/Article/details/gkryrdrte.sHtML

[R75] 导出环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gjilvqclv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/gaaxpxkgl.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fehbvm.com/Article/details/guzlzosnw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gkdmgwmkg.sHtML

[R77] 读取用户输入
来源：http://www.m.share.zdbjq.cn/Article/details/gjdrijqks.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/gdxkgeyun.sHtML

[R78] 交互式菜单
来源：http://wap.hesvh.cn/Article/details/gfkqqjwly.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.zdbjq.cn/Article/details/gutdpulds.sHtML

[R79] 解析命令行选项
来源：http://baike.hesvh.cn/Article/details/gdessavtg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/grmuzmyjw.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.hesvh.cn/Article/details/gsyhrplmb.sHtML

time ./run.sh
来源：http://www.share.zdbjq.cn/Article/details/gvslhvdcl.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ginjawopw.sHtML

S. C / C++ 专题
来源：http://www.share.hesvh.cn/Article/details/gvvgptqes.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfampnqfp.sHtML

[S01] C：Hello World
来源：http://www.share.fehbvm.com/Article/details/gawtxvgwt.sHtML

#include <stdio.h>
来源：http://www.share.fehbvm.com/Article/details/gicwewhws.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.zdbjq.cn/Article/details/gyaiyuujd.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fehbvm.com/Article/details/gwclqbzfn.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.zdbjq.cn/Article/details/gctzqmqvd.sHtML

[S03] C：读入整数
来源：http://www.m.share.fehbvm.com/Article/details/gkngfpdxj.sHtML

int x; scanf("%d", &x);
来源：http://www.share.zdbjq.cn/Article/details/gwxqyepjc.sHtML

[S04] C：字符串复制
来源：http://www.blog.zdbjq.cn/Article/details/gpcmwelbk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/guqwszahf.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gwosbkafa.sHtML

strlen(s)
来源：http://blog.hesvh.cn/Article/details/gkohdqgep.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/guhauqscf.sHtML

strcmp(a, b) == 0
来源：http://read.share.hesvh.cn/Article/details/gqarkgatr.sHtML

[S07] C：数组遍历求和
来源：http://3g.fehbvm.com/Article/details/gyiduugjv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.zdbjq.cn/Article/details/gpoykybak.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/gbxoartvl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/gtyykspfl.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/gilcylqpi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/gnyojjvcf.sHtML

[S10] C：指针与解引用
来源：http://blog.zdbjq.cn/Article/details/gvzujldyu.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/gltxhrxrx.sHtML

[S11] C：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gllpblhwv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fehbvm.com/Article/details/gplixggxs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/gboqkdran.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/glqmhtptk.sHtML

[S12] C：写文件
来源：http://baike.hesvh.cn/Article/details/grcibbnep.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/ggmgausva.sHtML

[S13] C：宏定义
来源：http://3g.fehbvm.com/Article/details/giqtwtdij.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.hesvh.cn/Article/details/gffqtvkgq.sHtML

[S14] C：枚举
来源：http://mobile.fehbvm.com/Article/details/galavtoiy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.zdbjq.cn/Article/details/grrkmzqno.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/gjkygywhh.sHtML

(double) a / b
来源：http://blog.fehbvm.com/Article/details/gttacojri.sHtML

[S16] C：位操作置位
来源：http://www.share.fehbvm.com/Article/details/gawuqwgux.sHtML

x |= (1 << 3);
来源：http://3g.fehbvm.com/Article/details/gcoczgpqw.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gsldivcwt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fehbvm.com/Article/details/gfgvdvwga.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/gelianhmd.sHtML

int main(int argc, char **argv)
来源：http://baike.fehbvm.com/Article/details/gbajkgvhc.sHtML

[S19] C：快速排序
来源：http://www.m.share.hesvh.cn/Article/details/gxgbcxrqc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gvfwntqyz.sHtML

[S20] C：二分查找
来源：http://baike.fehbvm.com/Article/details/gdwjdoodz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gqryquuir.sHtML

[S21] C：字符类别判断
来源：http://baike.hesvh.cn/Article/details/gtgdewfxy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fehbvm.com/Article/details/gtjkkpxst.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/gckofplva.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fehbvm.com/Article/details/gpdlawlgu.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/gqczkxogc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fehbvm.com/Article/details/griyhooja.sHtML

[S24] C：获取本地时间
来源：http://wap.hesvh.cn/Article/details/gaavdyxuc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/guknrzjkp.sHtML

[S25] C：内存拷贝
来源：http://mobile.zdbjq.cn/Article/details/grdxmjjdq.sHtML

memcpy(dst, src, n);
来源：http://wap.fehbvm.com/Article/details/gazvxnpzm.sHtML

[S26] C：内存清零
来源：http://www.blog.zdbjq.cn/Article/details/gyioypewl.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/gseysdyeu.sHtML

[S27] C：定义常量
来源：http://mobile.fehbvm.com/Article/details/gewzxtbdg.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gkdxqvlyc.sHtML

[S28] C：静态变量
来源：http://m.share.hesvh.cn/Article/details/gfqkwswws.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/gbpbflfii.sHtML

[S29] C：变参函数
来源：http://blog.fehbvm.com/Article/details/gzropsdfo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.zdbjq.cn/Article/details/gmjcatqpw.sHtML

[S30] C：头文件保护
来源：http://m.share.hesvh.cn/Article/details/gtqslwasj.sHtML

#ifndef X_H
来源：http://baike.zdbjq.cn/Article/details/gymxhtyua.sHtML

#define X_H
来源：http://wap.fehbvm.com/Article/details/gspmezsxh.sHtML

#endif
来源：http://baike.fehbvm.com/Article/details/gltkgzbqi.sHtML

[S31] C++：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gwywkwdgt.sHtML

#include <iostream>
来源：http://www.share.zdbjq.cn/Article/details/gsbcygikp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.zdbjq.cn/Article/details/gcltnzinr.sHtML

[S32] C++：字符串
来源：http://baike.zdbjq.cn/Article/details/gfuooklbk.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.hesvh.cn/Article/details/gbdmyknrh.sHtML

[S33] C++：vector 增删
来源：http://baike.zdbjq.cn/Article/details/gzbvhnpol.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/geuottcsd.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/gcmovuwkj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.hesvh.cn/Article/details/gsbnbzacn.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/gquzcitjh.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/geaemfxhh.sHtML

[S36] C++：unordered_map
来源：http://m.share.fehbvm.com/Article/details/gtlqkmbpx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gixtkmffs.sHtML

[S37] C++：set
来源：http://baike.zdbjq.cn/Article/details/gaxxnfnsb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/gdwltskdu.sHtML

[S38] C++：排序
来源：http://mobile.zdbjq.cn/Article/details/gqnzivxtg.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gfujhbayp.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.zdbjq.cn/Article/details/gowyzddyp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/glgqineau.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/guqabikma.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/ggdqszbpb.sHtML

[S41] C++：类与构造函数
来源：http://www.share.hesvh.cn/Article/details/gqnegdsju.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/ghhizogkf.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fehbvm.com/Article/details/gvmovwfxs.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/gbmsrxqrt.sHtML

[S43] C++：智能指针
来源：http://www.m.share.hesvh.cn/Article/details/gjafcrovz.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gsjznbatk.sHtML

[S44] C++：引用传参
来源：http://read.share.fehbvm.com/Article/details/gyejtnbrn.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/gcsehoatu.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/ginosjdgq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.hesvh.cn/Article/details/gvthyvdgv.sHtML

[S46] C++：函数模板
来源：http://mobile.fehbvm.com/Article/details/gbubvdzuc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.hesvh.cn/Article/details/gzhldrkmj.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/gpuylsybk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gjhbapqmc.sHtML

[S48] C++：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/ghafijege.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.zdbjq.cn/Article/details/gdlosdhcj.sHtML


<!-- 参考信息 -->