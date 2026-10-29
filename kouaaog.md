代发 wailian999

[Q82] 字符长度与字节长度
来源：http://blog.hesvh.cn/Article/details/gbwztzqyz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gtrlypivr.sHtML

[Q83] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gicyeuvfw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gelxurqhk.sHtML

[Q84] 去除首尾空格
来源：http://www.share.zdbjq.cn/Article/details/glijnlcyo.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gceatzfea.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/gdirmvcae.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.hesvh.cn/Article/details/gftvzdvum.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fehbvm.com/Article/details/gzpszuskt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.zdbjq.cn/Article/details/gcyzjxosb.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fehbvm.com/Article/details/geleustqi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/gdovorwkm.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.zdbjq.cn/Article/details/gbbvuvguj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fehbvm.com/Article/details/gtnkxijlp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gktddgzfw.sHtML

[Q89] 判断表是否存在
来源：http://blog.fehbvm.com/Article/details/gsemjngcp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.hesvh.cn/Article/details/gprdagdqw.sHtML

[Q90] 生成序号列
来源：http://m.share.hesvh.cn/Article/details/ganodcqiq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.hesvh.cn/Article/details/geioqgggx.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmusogzxm.sHtML

R. Bash 专题
来源：http://3g.fehbvm.com/Article/details/gmmpsmfdm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbcsdrjjt.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/gfwrwfeim.sHtML

#!/usr/bin/env bash
来源：http://baike.fehbvm.com/Article/details/gadylmbjr.sHtML

set -euo pipefail
来源：http://read.share.hesvh.cn/Article/details/gvuijmzmq.sHtML

[R02] 变量赋值与使用
来源：http://wap.hesvh.cn/Article/details/gsvfnvkax.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/gvctaxfmy.sHtML

[R03] 只读变量
来源：http://mobile.zdbjq.cn/Article/details/gzyqwlnyi.sHtML

readonly PI=3.14
来源：http://blog.hesvh.cn/Article/details/gzwxgiaos.sHtML

[R04] 位置参数
来源：http://3g.hesvh.cn/Article/details/gnbopxksv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.zdbjq.cn/Article/details/gxzgnnsra.sHtML

[R05] 参数默认值
来源：http://mobile.hesvh.cn/Article/details/gohikouks.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/gfzqrcskt.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fehbvm.com/Article/details/goaapcdko.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gchlbchog.sHtML

[R07] if 判断文件
来源：http://wap.fehbvm.com/Article/details/gqcksydfq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fehbvm.com/Article/details/gabnbokhj.sHtML

[R08] 数值比较
来源：http://wap.hesvh.cn/Article/details/gjtqnsjap.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.hesvh.cn/Article/details/gcsolomdj.sHtML

[R09] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/gutgmwurk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/greygyzpv.sHtML

[R10] 正则匹配
来源：http://mobile.fehbvm.com/Article/details/gxhxyzwpb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fehbvm.com/Article/details/gkmhaxkwd.sHtML

[R11] case 多分支
来源：http://www.m.share.hesvh.cn/Article/details/gzjhshbqv.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/gbdcazwey.sHtML

start) echo "启动" ;;
来源：http://mobile.fehbvm.com/Article/details/gwrlooznl.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/gadoweayi.sHtML

*)     echo "未知命令" ;;
来源：http://baike.zdbjq.cn/Article/details/gpqlrfblt.sHtML

esac
来源：http://baike.fehbvm.com/Article/details/gtvuergfn.sHtML

[R12] for 遍历文件
来源：http://3g.zdbjq.cn/Article/details/gsrtacqpy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.hesvh.cn/Article/details/gkjedzmsi.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/gxylwnsls.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gjulywzdh.sHtML

[R14] C 风格 for
来源：http://www.blog.fehbvm.com/Article/details/gspgflkwf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gtkgrgrgr.sHtML

[R15] while 逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gujwbfsow.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fehbvm.com/Article/details/gjkurwzlu.sHtML

[R16] until 等待条件
来源：http://m.share.hesvh.cn/Article/details/gbrovycmu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gejmefjyh.sHtML

[R17] 数组定义与取值
来源：http://blog.hesvh.cn/Article/details/ghzsveykl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.zdbjq.cn/Article/details/gmswnffdf.sHtML

[R18] 遍历数组
来源：http://www.blog.hesvh.cn/Article/details/gwmsvfydp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fehbvm.com/Article/details/gzlfnauze.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gcbrqqfeh.sHtML

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/gplutbiok.sHtML

[R20] 关联数组（字典）
来源：http://m.share.zdbjq.cn/Article/details/gkragtvsu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.zdbjq.cn/Article/details/gqcnplfgu.sHtML

[R21] 字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gezkhfhru.sHtML

echo "${#s}"
来源：http://www.m.share.zdbjq.cn/Article/details/gvnxhlohd.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gqybflpoh.sHtML

echo "${s:0:5}"
来源：http://m.share.hesvh.cn/Article/details/gvimpqeuz.sHtML

[R23] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gaypapadr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.zdbjq.cn/Article/details/gkypdezgp.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gzolevzhr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.hesvh.cn/Article/details/gbfkrimtd.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.hesvh.cn/Article/details/gvgdpqiuf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fehbvm.com/Article/details/ggmksgerf.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/gbtnyjnah.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fehbvm.com/Article/details/gajkzzfis.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/gshacazsh.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/gyfnspuzu.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/grqzlsivc.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fehbvm.com/Article/details/gdiuuzlbx.sHtML

[R29] 定义函数
来源：http://3g.fehbvm.com/Article/details/gmbmcbleo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.hesvh.cn/Article/details/gqfozajxf.sHtML

[R30] 函数返回状态码
来源：http://www.share.fehbvm.com/Article/details/gkcvfghwt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.hesvh.cn/Article/details/gnaujxgbi.sHtML

[R31] 局部变量
来源：http://read.share.hesvh.cn/Article/details/gfnmttwml.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/gnntxwnfh.sHtML

[R32] 参数个数校验
来源：http://www.blog.fehbvm.com/Article/details/gjdhomllc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gtbiqxtfk.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.zdbjq.cn/Article/details/gxiwogngt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/gmsdkocut.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/gqhnaotol.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gobvfxyqd.sHtML

[R35] 后台执行并等待
来源：http://wap.fehbvm.com/Article/details/ghjlgsxhc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fehbvm.com/Article/details/gljnekqpq.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/gsqghbyme.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.hesvh.cn/Article/details/guuqlzzzs.sHtML

[R37] 把输出赋给变量
来源：http://blog.fehbvm.com/Article/details/ggkyxivrh.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/gfqktvpfq.sHtML

[R38] 管道串联
来源：http://www.m.share.zdbjq.cn/Article/details/gwiysjzzw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/gqwuhzbtt.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/gvapwtnzx.sHtML

cmd > out.log 2>&1
来源：http://mobile.fehbvm.com/Article/details/gboviqnyz.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/glpnxjjse.sHtML

echo "log" >> out.log
来源：http://www.m.share.fehbvm.com/Article/details/gpzwckazb.sHtML

[R41] 丢弃输出
来源：http://www.share.fehbvm.com/Article/details/gsqcylpyb.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gkucslssj.sHtML

[R42] 输入重定向
来源：http://mobile.fehbvm.com/Article/details/gfsgkiiem.sHtML

wc -l < a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gavazbnji.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/gebpezdty.sHtML

find . -name "*.log" -type f
来源：http://read.share.hesvh.cn/Article/details/gdqvbvixc.sHtML

[R44] 按修改时间查找
来源：http://www.share.zdbjq.cn/Article/details/gaznbhfzt.sHtML

find . -mtime -7 -type f
来源：http://blog.hesvh.cn/Article/details/gtksqsosr.sHtML

[R45] 批量删除
来源：http://m.share.hesvh.cn/Article/details/gfdzhdvft.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fehbvm.com/Article/details/gdglfbvlf.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/gtzjngfqa.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fehbvm.com/Article/details/glhxsvrlp.sHtML

[R47] sed 单行替换
来源：http://baike.hesvh.cn/Article/details/gycgnonhv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/grcmzcbsh.sHtML

[R48] awk 取指定列
来源：http://www.blog.hesvh.cn/Article/details/gntilbuhh.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.hesvh.cn/Article/details/ghzjzznof.sHtML

[R49] awk 带条件
来源：http://www.blog.fehbvm.com/Article/details/gwgxmktws.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fehbvm.com/Article/details/gpmffcuig.sHtML

[R50] awk 求和
来源：http://wap.zdbjq.cn/Article/details/gxwgpcyqv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gpzxenbrs.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fehbvm.com/Article/details/gtfyeiapr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.hesvh.cn/Article/details/ggbpaeuik.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/gpmxywqdl.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/gscijrtyj.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/ggpzysrbi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fehbvm.com/Article/details/gyvcgwdqp.sHtML

[R54] 比较两个文件
来源：http://wap.zdbjq.cn/Article/details/gbequuggy.sHtML

diff a.txt b.txt
来源：http://mobile.fehbvm.com/Article/details/gnfxwnxew.sHtML

[R55] 压缩与解压
来源：http://3g.fehbvm.com/Article/details/gmyjjqmeu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/gofbchmbd.sHtML

[R56] 远程拷贝
来源：http://read.share.hesvh.cn/Article/details/galjcvywa.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/gtnbcgscv.sHtML

[R57] 远程执行命令
来源：http://mobile.fehbvm.com/Article/details/ghgfgumuc.sHtML

ssh user@host 'uptime'
来源：http://mobile.fehbvm.com/Article/details/gpyrwssmb.sHtML

[R58] 下载文件
来源：http://baike.hesvh.cn/Article/details/ggflnoocy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fehbvm.com/Article/details/gohvkkcwp.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/gdwqfzrkn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.zdbjq.cn/Article/details/ghwtwspib.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gothqjcpr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.zdbjq.cn/Article/details/gcwrizfzf.sHtML

[R61] 磁盘占用
来源：http://wap.fehbvm.com/Article/details/gzwqfxpjk.sHtML

df -h;  du -sh *
来源：http://m.share.fehbvm.com/Article/details/ghwzszvcs.sHtML

[R62] 找最占空间的文件
来源：http://baike.zdbjq.cn/Article/details/gnsrybrom.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fehbvm.com/Article/details/gxbjnohny.sHtML

[R63] 内存与进程
来源：http://mobile.zdbjq.cn/Article/details/grfdhshtk.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fehbvm.com/Article/details/geuqornli.sHtML

[R64] 结束进程
来源：http://read.share.zdbjq.cn/Article/details/gbuaxttor.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.zdbjq.cn/Article/details/guwokdmsz.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gpwxgripf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fehbvm.com/Article/details/gqwynyxqw.sHtML

[R66] 定时任务
来源：http://3g.hesvh.cn/Article/details/gwecplryg.sHtML

crontab -e;  crontab -l
来源：http://wap.fehbvm.com/Article/details/geymcbjeg.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/ggsqjhucv.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/gweuuviov.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/gbkrbgjhq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.hesvh.cn/Article/details/grufqqdph.sHtML

[R69] 生成随机密码
来源：http://read.share.hesvh.cn/Article/details/gahncnrrh.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fehbvm.com/Article/details/gwcjmnrja.sHtML

[R70] 时间戳与互转
来源：http://mobile.zdbjq.cn/Article/details/gohzabavt.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fehbvm.com/Article/details/gulevjovw.sHtML

[R71] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/glbtwdpme.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.hesvh.cn/Article/details/gjhbrjtrb.sHtML

[R72] 等待端口就绪
来源：http://3g.hesvh.cn/Article/details/gtgiacadr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gndynyldf.sHtML

[R73] 分割大日志
来源：http://wap.zdbjq.cn/Article/details/grffiniue.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/grgsqvwrj.sHtML

[R74] 批量重命名
来源：http://m.share.fehbvm.com/Article/details/gkwfoohha.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fehbvm.com/Article/details/gezrsnzwt.sHtML

[R75] 导出环境变量
来源：http://read.share.zdbjq.cn/Article/details/gxleekhen.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.hesvh.cn/Article/details/gnnexfzyd.sHtML

[R76] 使用临时文件
来源：http://www.blog.hesvh.cn/Article/details/gtgepmhoq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gijnhtubh.sHtML

[R77] 读取用户输入
来源：http://baike.zdbjq.cn/Article/details/gbztibfaa.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/gknjfmshs.sHtML

[R78] 交互式菜单
来源：http://3g.hesvh.cn/Article/details/gcvhyksbq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/geqbqqlml.sHtML

[R79] 解析命令行选项
来源：http://www.share.fehbvm.com/Article/details/giotpxkgn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.zdbjq.cn/Article/details/gwlmtxazj.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fehbvm.com/Article/details/gubvraxay.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/gbqnmpkrj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqmxbzxre.sHtML

S. C / C++ 专题
来源：http://3g.hesvh.cn/Article/details/gqnsujrly.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbkizfysm.sHtML

[S01] C：Hello World
来源：http://3g.zdbjq.cn/Article/details/gqxskqxeq.sHtML

#include <stdio.h>
来源：http://read.share.hesvh.cn/Article/details/gkgeefbwk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/gxvbhezbc.sHtML

[S02] C：变量与格式化输出
来源：http://3g.zdbjq.cn/Article/details/gzojricir.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.hesvh.cn/Article/details/gesenodms.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/gcendlfdo.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/gpdoznxlo.sHtML

[S04] C：字符串复制
来源：http://read.share.fehbvm.com/Article/details/gaospzyot.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/gyiultmnv.sHtML

[S05] C：字符串长度
来源：http://m.share.fehbvm.com/Article/details/gvpgztnfk.sHtML

strlen(s)
来源：http://blog.fehbvm.com/Article/details/gwlhlgpko.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gelrngrvp.sHtML

strcmp(a, b) == 0
来源：http://blog.fehbvm.com/Article/details/gpdcnixmi.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.hesvh.cn/Article/details/guoutitfw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.zdbjq.cn/Article/details/gecvmgkjt.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.zdbjq.cn/Article/details/gycoawcmv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/gwbquzgaf.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fehbvm.com/Article/details/gkuhwhymi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.hesvh.cn/Article/details/gsoohggqc.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gxdxxegcd.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.hesvh.cn/Article/details/goyebtapu.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gpxbunfdx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.hesvh.cn/Article/details/gdlpxatoj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gbjeffnov.sHtML

fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/ghyeczxxy.sHtML

[S12] C：写文件
来源：http://blog.hesvh.cn/Article/details/gkxeprovw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gemzgeyrm.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/gomounpdi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/gfhuseahu.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/gkdkuuifq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fehbvm.com/Article/details/gycxaeuec.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/gmdygpiaq.sHtML

(double) a / b
来源：http://blog.zdbjq.cn/Article/details/glepaenmn.sHtML

[S16] C：位操作置位
来源：http://mobile.hesvh.cn/Article/details/gytfrezsi.sHtML

x |= (1 << 3);
来源：http://mobile.fehbvm.com/Article/details/gdtapoouf.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.hesvh.cn/Article/details/goesaorpq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fehbvm.com/Article/details/gxddexmqu.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/gjlzoxboq.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/gwbroopsg.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/gugbrgtyc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/goeqajzah.sHtML

[S20] C：二分查找
来源：http://mobile.hesvh.cn/Article/details/gopqfwcfw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gtdobbplo.sHtML

[S21] C：字符类别判断
来源：http://read.share.fehbvm.com/Article/details/gfiwozazj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/ggyplopia.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/ghjpyvoxh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/goxdkxrjs.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/grkzyuhsn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.hesvh.cn/Article/details/gdnmfcfrb.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/gwodngcss.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.hesvh.cn/Article/details/ghzxfzmyu.sHtML

[S25] C：内存拷贝
来源：http://3g.hesvh.cn/Article/details/gltrprkqw.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/gjvylrwkx.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/giarjgtrj.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/gvtcddakw.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/gxglzthna.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/ghvdpundb.sHtML

[S28] C：静态变量
来源：http://3g.hesvh.cn/Article/details/gxzpjblqq.sHtML

static int counter = 0;
来源：http://baike.zdbjq.cn/Article/details/glkmyufao.sHtML

[S29] C：变参函数
来源：http://baike.hesvh.cn/Article/details/gnyxkmnko.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/gmgkdljix.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/gqxguhavn.sHtML

#ifndef X_H
来源：http://read.share.zdbjq.cn/Article/details/gyvxbwist.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/gxkqxqrjc.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/gcxootqwr.sHtML

[S31] C++：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gbfjsclqe.sHtML

#include <iostream>
来源：http://wap.fehbvm.com/Article/details/gfupuxyaf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fehbvm.com/Article/details/gkcvsnsvi.sHtML

[S32] C++：字符串
来源：http://blog.fehbvm.com/Article/details/ggreealbf.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.hesvh.cn/Article/details/gfpjksxdp.sHtML

[S33] C++：vector 增删
来源：http://m.share.hesvh.cn/Article/details/gczdkwaqw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.hesvh.cn/Article/details/gkydxakvb.sHtML

[S34] C++：遍历 vector
来源：http://wap.zdbjq.cn/Article/details/gumibbopz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/gkhopirxz.sHtML

[S35] C++：map
来源：http://wap.hesvh.cn/Article/details/gquuyqwfg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gqdwsuuhl.sHtML

[S36] C++：unordered_map
来源：http://3g.hesvh.cn/Article/details/gonckpbxy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gmwrtdjzl.sHtML

[S37] C++：set
来源：http://blog.zdbjq.cn/Article/details/getdzambk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.zdbjq.cn/Article/details/guqkyblgi.sHtML

[S38] C++：排序
来源：http://www.blog.hesvh.cn/Article/details/gnugycxzs.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.zdbjq.cn/Article/details/grgasrlny.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/ghxrptfsp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.zdbjq.cn/Article/details/gnirymdpj.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fehbvm.com/Article/details/glibrxafm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.hesvh.cn/Article/details/gkwvwzwht.sHtML

[S41] C++：类与构造函数
来源：http://baike.hesvh.cn/Article/details/gnlecjszs.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.zdbjq.cn/Article/details/gpqoopzqr.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fehbvm.com/Article/details/gxsodipdl.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fehbvm.com/Article/details/gixnyjsmp.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/gxwsxhcsd.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/gwyjsqpyp.sHtML

[S44] C++：引用传参
来源：http://3g.hesvh.cn/Article/details/grbrrfdnf.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fehbvm.com/Article/details/gbomwiooo.sHtML

[S45] C++：lambda
来源：http://blog.hesvh.cn/Article/details/gmiumawen.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.zdbjq.cn/Article/details/gbhtnmpvz.sHtML

[S46] C++：函数模板
来源：http://read.share.fehbvm.com/Article/details/gguulyrdx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fehbvm.com/Article/details/gqccgkejm.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fehbvm.com/Article/details/ggzwjvdhc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.zdbjq.cn/Article/details/gxwkhpafp.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gzvqfzukr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/goapglxsc.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/grpkqrzfq.sHtML

[S49] C++：写文件
来源：http://www.share.fehbvm.com/Article/details/grslqbfti.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.hesvh.cn/Article/details/gscqytstl.sHtML

[S50] C++：格式化数字
来源：http://wap.hesvh.cn/Article/details/gzxagbhaz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.hesvh.cn/Article/details/gbpsvolbp.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/gkkkndluc.sHtML

static_cast<double>(a) / b
来源：http://m.share.hesvh.cn/Article/details/ggmtxnpty.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.zdbjq.cn/Article/details/glpwnpbne.sHtML


<!-- 参考信息 -->