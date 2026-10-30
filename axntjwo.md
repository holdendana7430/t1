代发 wailian999

[Q78] 当前时间
来源：http://blog.hesvh.cn/Article/details/gftfourjp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fehbvm.com/Article/details/gbxaihjxe.sHtML

[Q79] 字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gpiwowxdo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fehbvm.com/Article/details/grzsdybrb.sHtML

[Q80] 字符串截取
来源：http://blog.zdbjq.cn/Article/details/gzgmsiqql.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gkcqjftse.sHtML

[Q81] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gusqtyauj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.hesvh.cn/Article/details/gvtjkbkwg.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.hesvh.cn/Article/details/gummwpxzq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gfdtbgewd.sHtML

[Q83] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gqaeibtqn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/glxpmbeem.sHtML

[Q84] 去除首尾空格
来源：http://mobile.zdbjq.cn/Article/details/gmstvzgsc.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gzpvflqau.sHtML

[Q85] 数值取整
来源：http://m.share.zdbjq.cn/Article/details/geonjdkte.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fehbvm.com/Article/details/gijjwguyj.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.zdbjq.cn/Article/details/gpstdcfuz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/gmkvukkzs.sHtML

[Q87] JSON 字段做条件
来源：http://blog.hesvh.cn/Article/details/glzomdoqz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.hesvh.cn/Article/details/gzvimabtu.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fehbvm.com/Article/details/gcjeczmfx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fehbvm.com/Article/details/gwickjvpa.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/gegluudmg.sHtML

[Q89] 判断表是否存在
来源：http://wap.hesvh.cn/Article/details/gtiutsuvp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fehbvm.com/Article/details/gxpwfawpl.sHtML

[Q90] 生成序号列
来源：http://mobile.hesvh.cn/Article/details/gjuphjnjt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/gxpawoxgi.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjkycswlg.sHtML

R. Bash 专题
来源：http://wap.fehbvm.com/Article/details/ghshusdjd.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gutgpzwtu.sHtML

[R01] shebang 与严格模式
来源：http://mobile.zdbjq.cn/Article/details/glvnmtdkm.sHtML

#!/usr/bin/env bash
来源：http://baike.zdbjq.cn/Article/details/gecjcdnil.sHtML

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/gundctcbp.sHtML

[R02] 变量赋值与使用
来源：http://3g.hesvh.cn/Article/details/gslytkasb.sHtML

name="Tom"; echo "$name"
来源：http://3g.fehbvm.com/Article/details/gumblvnow.sHtML

[R03] 只读变量
来源：http://blog.fehbvm.com/Article/details/gkyixmwcf.sHtML

readonly PI=3.14
来源：http://mobile.hesvh.cn/Article/details/gvztmlgoy.sHtML

[R04] 位置参数
来源：http://3g.fehbvm.com/Article/details/glmwlnlgq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.zdbjq.cn/Article/details/gipjnwigv.sHtML

[R05] 参数默认值
来源：http://www.m.share.hesvh.cn/Article/details/gnpnwwztl.sHtML

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/gfnyyiody.sHtML

[R06] 判断命令是否存在
来源：http://read.share.zdbjq.cn/Article/details/gysbexqaa.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gqmakprep.sHtML

[R07] if 判断文件
来源：http://baike.hesvh.cn/Article/details/gvvvdfobf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.zdbjq.cn/Article/details/ghgvxcovq.sHtML

[R08] 数值比较
来源：http://m.share.hesvh.cn/Article/details/gfngemzmf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.hesvh.cn/Article/details/guizditeq.sHtML

[R09] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/gwoofxpdz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gymrjpjsg.sHtML

[R10] 正则匹配
来源：http://www.m.share.fehbvm.com/Article/details/geldqgstw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/grumzzdkg.sHtML

[R11] case 多分支
来源：http://3g.hesvh.cn/Article/details/gsoozfndv.sHtML

case "$1" in
来源：http://baike.hesvh.cn/Article/details/gsavnbzmu.sHtML

start) echo "启动" ;;
来源：http://www.blog.fehbvm.com/Article/details/gboehlnrr.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fehbvm.com/Article/details/gjeksilam.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.hesvh.cn/Article/details/grqcwcwtj.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/gpsvdpsrh.sHtML

[R12] for 遍历文件
来源：http://m.share.zdbjq.cn/Article/details/glwerjlzq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fehbvm.com/Article/details/gisfidzmn.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/ghrajfpgq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/ghyxnmhgv.sHtML

[R14] C 风格 for
来源：http://www.m.share.hesvh.cn/Article/details/gedcdrmvt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gpadgbxpg.sHtML

[R15] while 逐行读文件
来源：http://wap.fehbvm.com/Article/details/gsmfzyobg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fehbvm.com/Article/details/gdkijhczp.sHtML

[R16] until 等待条件
来源：http://mobile.fehbvm.com/Article/details/geebenwnx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gpbhfkzcm.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/gwwesgjhg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.hesvh.cn/Article/details/gwpdzdvwn.sHtML

[R18] 遍历数组
来源：http://www.m.share.zdbjq.cn/Article/details/gchdppixj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/gvjrttzlp.sHtML

[R19] 数组长度
来源：http://baike.hesvh.cn/Article/details/gqycroqus.sHtML

echo "${#arr[@]}"
来源：http://mobile.fehbvm.com/Article/details/gosikivrx.sHtML

[R20] 关联数组（字典）
来源：http://3g.hesvh.cn/Article/details/gkpesdpgw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fehbvm.com/Article/details/gehhfnhek.sHtML

[R21] 字符串长度
来源：http://blog.zdbjq.cn/Article/details/ghsrnwrtz.sHtML

echo "${#s}"
来源：http://3g.hesvh.cn/Article/details/gaukpdzlq.sHtML

[R22] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gqtqklceu.sHtML

echo "${s:0:5}"
来源：http://www.share.fehbvm.com/Article/details/gjxpyfjxu.sHtML

[R23] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gyvvubbhp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fehbvm.com/Article/details/gbronliry.sHtML

[R24] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gzuxgwxdd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fehbvm.com/Article/details/gxzmcucse.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fehbvm.com/Article/details/gtclyexvn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.zdbjq.cn/Article/details/gptsgftpr.sHtML

[R26] 命令替换
来源：http://www.blog.hesvh.cn/Article/details/gnhnijtyz.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.zdbjq.cn/Article/details/gcqrctwfm.sHtML

[R27] 算术展开
来源：http://3g.fehbvm.com/Article/details/giufzkrde.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fehbvm.com/Article/details/gwrpcddsj.sHtML

[R28] 浮点运算
来源：http://blog.zdbjq.cn/Article/details/gidbouhof.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fehbvm.com/Article/details/gvhmennhi.sHtML

[R29] 定义函数
来源：http://3g.hesvh.cn/Article/details/gwqvzemcp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.hesvh.cn/Article/details/gvrfebxvn.sHtML

[R30] 函数返回状态码
来源：http://www.share.fehbvm.com/Article/details/guivhssge.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.hesvh.cn/Article/details/gojnxsrsj.sHtML

[R31] 局部变量
来源：http://wap.fehbvm.com/Article/details/gzndamvaf.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.zdbjq.cn/Article/details/gtxqhakho.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/gvlojtpae.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gcorbejaj.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fehbvm.com/Article/details/gjfzwaayd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fehbvm.com/Article/details/gajhlzqxe.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/gjzabdfya.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gsvyrsdyq.sHtML

[R35] 后台执行并等待
来源：http://3g.fehbvm.com/Article/details/gkvvvldct.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/gvhnafpcp.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.hesvh.cn/Article/details/gicxvmkfv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.zdbjq.cn/Article/details/gxtnhsqcm.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/gqssninez.sHtML

files=$(ls -1)
来源：http://wap.zdbjq.cn/Article/details/gjsftqnzq.sHtML

[R38] 管道串联
来源：http://www.blog.hesvh.cn/Article/details/guohsyjnr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/gmhocgbqy.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.zdbjq.cn/Article/details/gowviutcc.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gdfvzrwmi.sHtML

[R40] 追加写日志
来源：http://wap.zdbjq.cn/Article/details/gnmpwdjax.sHtML

echo "log" >> out.log
来源：http://3g.hesvh.cn/Article/details/gaoofuxmu.sHtML

[R41] 丢弃输出
来源：http://3g.zdbjq.cn/Article/details/ghrpkjolz.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.hesvh.cn/Article/details/gdzntwnix.sHtML

[R42] 输入重定向
来源：http://baike.zdbjq.cn/Article/details/gqijpmzct.sHtML

wc -l < a.txt
来源：http://www.share.zdbjq.cn/Article/details/gjkhofltv.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/gqysknqem.sHtML

find . -name "*.log" -type f
来源：http://3g.hesvh.cn/Article/details/gyhmdzkea.sHtML

[R44] 按修改时间查找
来源：http://wap.zdbjq.cn/Article/details/gwbggqtms.sHtML

find . -mtime -7 -type f
来源：http://mobile.fehbvm.com/Article/details/gqtzyuouu.sHtML

[R45] 批量删除
来源：http://blog.hesvh.cn/Article/details/glplvervz.sHtML

find . -name "*.tmp" -delete
来源：http://baike.hesvh.cn/Article/details/gocqawmzi.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/grupopjom.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.zdbjq.cn/Article/details/gicudvdwi.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/ggaazgezt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gwxmcazco.sHtML

[R48] awk 取指定列
来源：http://blog.fehbvm.com/Article/details/gszsjwjmf.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/glakphbwk.sHtML

[R49] awk 带条件
来源：http://baike.zdbjq.cn/Article/details/gioeidwky.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.zdbjq.cn/Article/details/gthibnwnc.sHtML

[R50] awk 求和
来源：http://wap.zdbjq.cn/Article/details/gxfrmeloq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gcdggrmvv.sHtML

[R51] 排序去重取前几
来源：http://wap.zdbjq.cn/Article/details/gihaxqloo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/goryhyvei.sHtML

[R52] 统计行数
来源：http://www.m.share.hesvh.cn/Article/details/glkewyurz.sHtML

wc -l a.txt
来源：http://3g.zdbjq.cn/Article/details/ghgqozxbc.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/guzfxvdmm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.zdbjq.cn/Article/details/grxzzjbcz.sHtML

[R54] 比较两个文件
来源：http://baike.zdbjq.cn/Article/details/gxrvimdsa.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/glswcwxip.sHtML

[R55] 压缩与解压
来源：http://www.m.share.zdbjq.cn/Article/details/gxaifewof.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fehbvm.com/Article/details/gseqanpng.sHtML

[R56] 远程拷贝
来源：http://wap.fehbvm.com/Article/details/gbqdzfeoj.sHtML

scp file user@host:/path/
来源：http://baike.hesvh.cn/Article/details/gbdompbsb.sHtML

[R57] 远程执行命令
来源：http://www.blog.zdbjq.cn/Article/details/gsthwkzde.sHtML

ssh user@host 'uptime'
来源：http://m.share.hesvh.cn/Article/details/gyralwxrr.sHtML

[R58] 下载文件
来源：http://read.share.fehbvm.com/Article/details/gtrvflnxm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fehbvm.com/Article/details/garigkyjs.sHtML

[R59] 发 POST JSON
来源：http://wap.hesvh.cn/Article/details/ghunthsra.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.hesvh.cn/Article/details/gdxfhsqgg.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gpdarbytx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/greyibttn.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/gfgnkuxtb.sHtML

df -h;  du -sh *
来源：http://read.share.fehbvm.com/Article/details/gbztvuqus.sHtML

[R62] 找最占空间的文件
来源：http://baike.zdbjq.cn/Article/details/gscnzrnwv.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.hesvh.cn/Article/details/gehpwfbda.sHtML

[R63] 内存与进程
来源：http://www.m.share.hesvh.cn/Article/details/gjntmxqts.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.zdbjq.cn/Article/details/gybimbomy.sHtML

[R64] 结束进程
来源：http://read.share.zdbjq.cn/Article/details/gqaohrqyu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fehbvm.com/Article/details/gtbydwgan.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/goxkvcgss.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fehbvm.com/Article/details/gmriqvqmh.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/gtpzejlfm.sHtML

crontab -e;  crontab -l
来源：http://baike.hesvh.cn/Article/details/gfvezqvol.sHtML

[R67] 生成随机十六进制串
来源：http://wap.zdbjq.cn/Article/details/gymguccxx.sHtML

openssl rand -hex 16
来源：http://mobile.zdbjq.cn/Article/details/grqavfqdh.sHtML

[R68] 计算文件校验值
来源：http://mobile.zdbjq.cn/Article/details/gbrhkbfwa.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/ghyijmxze.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/ggpcgpwiw.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fehbvm.com/Article/details/gnxbbdphp.sHtML

[R70] 时间戳与互转
来源：http://m.share.fehbvm.com/Article/details/gjdwsswng.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fehbvm.com/Article/details/glwbvhuzs.sHtML

[R71] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gmcaecang.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.zdbjq.cn/Article/details/gnsqditky.sHtML

[R72] 等待端口就绪
来源：http://wap.hesvh.cn/Article/details/grbmwfatf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/guewhdiwb.sHtML

[R73] 分割大日志
来源：http://wap.zdbjq.cn/Article/details/gziecqntk.sHtML

split -l 1000 big.log part_
来源：http://blog.hesvh.cn/Article/details/gdlsonzgb.sHtML

[R74] 批量重命名
来源：http://blog.hesvh.cn/Article/details/gmqoohogm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.hesvh.cn/Article/details/gskjnubpp.sHtML

[R75] 导出环境变量
来源：http://mobile.hesvh.cn/Article/details/gtkngpkfv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fehbvm.com/Article/details/gmmchakpr.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/gfndfaszs.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gmphejtcb.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/gqmpwofpx.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.hesvh.cn/Article/details/gqggvtsil.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/ggmndijal.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fehbvm.com/Article/details/gqpgvcpsy.sHtML

[R79] 解析命令行选项
来源：http://baike.hesvh.cn/Article/details/gyyuieywe.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.hesvh.cn/Article/details/gvdxozpka.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.hesvh.cn/Article/details/gtnlhpgje.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/gcotcsgap.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gveplpafb.sHtML

S. C / C++ 专题
来源：http://www.share.zdbjq.cn/Article/details/ggjvapsdq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gnkktclrm.sHtML

[S01] C：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gmorfamci.sHtML

#include <stdio.h>
来源：http://read.share.zdbjq.cn/Article/details/gnajumwux.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.zdbjq.cn/Article/details/gvcvlskqo.sHtML

[S02] C：变量与格式化输出
来源：http://baike.hesvh.cn/Article/details/ggparomyp.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fehbvm.com/Article/details/gxilvvocm.sHtML

[S03] C：读入整数
来源：http://www.blog.fehbvm.com/Article/details/gdmajwrir.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/gemeutmrf.sHtML

[S04] C：字符串复制
来源：http://www.blog.zdbjq.cn/Article/details/gvukihdxu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gaoyvebbv.sHtML

[S05] C：字符串长度
来源：http://baike.fehbvm.com/Article/details/gnngkfndc.sHtML

strlen(s)
来源：http://www.share.zdbjq.cn/Article/details/gxgchphuf.sHtML

[S06] C：字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gwadkjrsk.sHtML

strcmp(a, b) == 0
来源：http://m.share.hesvh.cn/Article/details/geaicecrw.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/gglhlcrsd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fehbvm.com/Article/details/gsehuiqco.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.zdbjq.cn/Article/details/godezuegg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/gwltwgocr.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.zdbjq.cn/Article/details/glixynrgv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/giwvhcels.sHtML

[S10] C：指针与解引用
来源：http://mobile.fehbvm.com/Article/details/gpzcqcjni.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.hesvh.cn/Article/details/gffhnwivb.sHtML

[S11] C：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gbnfgwglg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.hesvh.cn/Article/details/glvpkrrbz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fehbvm.com/Article/details/grspooqhl.sHtML

fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gdxsuhtsz.sHtML

[S12] C：写文件
来源：http://baike.hesvh.cn/Article/details/gjcymyloo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gcdkeuuiz.sHtML

[S13] C：宏定义
来源：http://www.m.share.fehbvm.com/Article/details/gcubqhgip.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fehbvm.com/Article/details/gnvaanbkg.sHtML

[S14] C：枚举
来源：http://m.share.fehbvm.com/Article/details/gvfskavaf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/guchwmuhs.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/gfkexwdpx.sHtML

(double) a / b
来源：http://baike.hesvh.cn/Article/details/gjvsumbvq.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/gcesaiglj.sHtML

x |= (1 << 3);
来源：http://www.share.hesvh.cn/Article/details/gjpdqpsmq.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fehbvm.com/Article/details/gdsgvltfx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.hesvh.cn/Article/details/guejdziyv.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/gjgxulvlp.sHtML

int main(int argc, char **argv)
来源：http://wap.zdbjq.cn/Article/details/gwiwbgarz.sHtML

[S19] C：快速排序
来源：http://www.m.share.hesvh.cn/Article/details/gfecyqdzq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/graesfbag.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/gtjclztpf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/ghurybvwq.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/girvpdjej.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/gkwwegvxa.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/gtlqecrcu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.zdbjq.cn/Article/details/gmevyohpw.sHtML

[S23] C：随机数
来源：http://www.blog.fehbvm.com/Article/details/gbhmrrsue.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.hesvh.cn/Article/details/gpsghsfvl.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/gtoatmqcz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fehbvm.com/Article/details/gajlgwbbr.sHtML

[S25] C：内存拷贝
来源：http://www.share.zdbjq.cn/Article/details/gyrgibzno.sHtML

memcpy(dst, src, n);
来源：http://read.share.hesvh.cn/Article/details/gpytcrkwi.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/gsmdtczbe.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fehbvm.com/Article/details/gmyvzljua.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/gtcbitibf.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gxwlqeydb.sHtML

[S28] C：静态变量
来源：http://blog.hesvh.cn/Article/details/gbvownrxh.sHtML

static int counter = 0;
来源：http://www.share.hesvh.cn/Article/details/ghridsfdm.sHtML

[S29] C：变参函数
来源：http://m.share.zdbjq.cn/Article/details/gsexbmufi.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fehbvm.com/Article/details/grezviwmy.sHtML

[S30] C：头文件保护
来源：http://www.blog.hesvh.cn/Article/details/gpnrioqsq.sHtML

#ifndef X_H
来源：http://baike.hesvh.cn/Article/details/gtqqtzjhf.sHtML

#define X_H
来源：http://www.blog.hesvh.cn/Article/details/gvnpbnioa.sHtML

#endif
来源：http://mobile.zdbjq.cn/Article/details/gegcbmyyb.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gngfcqulk.sHtML

#include <iostream>
来源：http://m.share.zdbjq.cn/Article/details/gbhmsxncb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.zdbjq.cn/Article/details/gzemwhfxg.sHtML

[S32] C++：字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gsaliyjmv.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fehbvm.com/Article/details/gzflgtmbh.sHtML

[S33] C++：vector 增删
来源：http://3g.zdbjq.cn/Article/details/gyoqomhay.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.zdbjq.cn/Article/details/gatboxoms.sHtML

[S34] C++：遍历 vector
来源：http://3g.zdbjq.cn/Article/details/gebdryqzk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.zdbjq.cn/Article/details/gumhmkmrf.sHtML

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/gxfzbiuaq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gvyxttpjy.sHtML

[S36] C++：unordered_map
来源：http://mobile.zdbjq.cn/Article/details/gxssyzfby.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gyzjubxsn.sHtML

[S37] C++：set
来源：http://www.share.zdbjq.cn/Article/details/gkvhzpemg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.zdbjq.cn/Article/details/glxvmoabb.sHtML

[S38] C++：排序
来源：http://www.m.share.zdbjq.cn/Article/details/gvwsttltd.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.hesvh.cn/Article/details/gyhrknepq.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.hesvh.cn/Article/details/gupwkvjfh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/gpvhmptcx.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/guajdnhkj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.zdbjq.cn/Article/details/grqfrsvha.sHtML

[S41] C++：类与构造函数
来源：http://m.share.zdbjq.cn/Article/details/gvnotupoh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/grxadzqft.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.zdbjq.cn/Article/details/ghulnqale.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.zdbjq.cn/Article/details/gftawtanz.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gqbefcfin.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/gtlpysuoo.sHtML

[S44] C++：引用传参
来源：http://blog.hesvh.cn/Article/details/geyhjveus.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fehbvm.com/Article/details/ggilqawlm.sHtML

[S45] C++：lambda
来源：http://www.blog.hesvh.cn/Article/details/gubdgxard.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.hesvh.cn/Article/details/gcsjwsqyg.sHtML

[S46] C++：函数模板
来源：http://wap.hesvh.cn/Article/details/gteqasjfj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/gbwefnuti.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.hesvh.cn/Article/details/gsontbasa.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.zdbjq.cn/Article/details/gveyakzyp.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gegnckqbf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/gdacttwid.sHtML


<!-- 参考信息 -->