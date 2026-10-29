代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fehbvm.com/Article/details/gaywzpqrv.sHtML

[Q75] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gnxojnvvc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gxhxegxam.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.zdbjq.cn/Article/details/gganyhuqx.sHtML

[Q76] 按天统计
来源：http://www.blog.zdbjq.cn/Article/details/geehamjyv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.hesvh.cn/Article/details/gzkdwezza.sHtML

[Q77] 时间加减
来源：http://3g.fehbvm.com/Article/details/gdarxofsd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.hesvh.cn/Article/details/gidiuwklj.sHtML

[Q78] 当前时间
来源：http://baike.hesvh.cn/Article/details/gyqxtrvzx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/gtrzjbcmw.sHtML

[Q79] 字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gfeauijld.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.zdbjq.cn/Article/details/girqrihkv.sHtML

[Q80] 字符串截取
来源：http://www.blog.hesvh.cn/Article/details/gvhvycbtb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fehbvm.com/Article/details/gcewcdwco.sHtML

[Q81] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gcbrwqzgw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gzqpkzwjw.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.hesvh.cn/Article/details/gpdknmson.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/giicpofwa.sHtML

[Q83] 大小写转换
来源：http://3g.hesvh.cn/Article/details/ghmcmzmbd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gnzzmepaz.sHtML

[Q84] 去除首尾空格
来源：http://baike.fehbvm.com/Article/details/gwbdbhuys.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gfwtgpnew.sHtML

[Q85] 数值取整
来源：http://www.m.share.zdbjq.cn/Article/details/gxupsdxaz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.hesvh.cn/Article/details/gssjojvub.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.hesvh.cn/Article/details/gdnracpcj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.zdbjq.cn/Article/details/gvbstmthd.sHtML

[Q87] JSON 字段做条件
来源：http://wap.hesvh.cn/Article/details/gfcbtswsi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.zdbjq.cn/Article/details/gxohodpkg.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.hesvh.cn/Article/details/ghedwyvta.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.hesvh.cn/Article/details/gmsruesht.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gjxuunnul.sHtML

[Q89] 判断表是否存在
来源：http://baike.zdbjq.cn/Article/details/gpxavlsxl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.zdbjq.cn/Article/details/glroiuuqu.sHtML

[Q90] 生成序号列
来源：http://mobile.fehbvm.com/Article/details/gbirpiqqw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fehbvm.com/Article/details/gonwbycmu.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gurqkugjb.sHtML

R. Bash 专题
来源：http://blog.fehbvm.com/Article/details/geczrbyjh.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwxgsqzet.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fehbvm.com/Article/details/gurwkgall.sHtML

#!/usr/bin/env bash
来源：http://read.share.zdbjq.cn/Article/details/grfzwwfaa.sHtML

set -euo pipefail
来源：http://m.share.hesvh.cn/Article/details/gppomxmiv.sHtML

[R02] 变量赋值与使用
来源：http://mobile.zdbjq.cn/Article/details/gksrmobbc.sHtML

name="Tom"; echo "$name"
来源：http://blog.hesvh.cn/Article/details/gryqadyyk.sHtML

[R03] 只读变量
来源：http://m.share.fehbvm.com/Article/details/ghjlktfzi.sHtML

readonly PI=3.14
来源：http://m.share.zdbjq.cn/Article/details/gcxodnlmk.sHtML

[R04] 位置参数
来源：http://mobile.fehbvm.com/Article/details/gdurdhcrp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/gubspgrzl.sHtML

[R05] 参数默认值
来源：http://baike.hesvh.cn/Article/details/grpviaild.sHtML

name="${1:-default}"
来源：http://read.share.hesvh.cn/Article/details/ggkmjljie.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fehbvm.com/Article/details/gwwehrmgv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gupqzcxhl.sHtML

[R07] if 判断文件
来源：http://www.m.share.fehbvm.com/Article/details/gutidnvit.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.zdbjq.cn/Article/details/gudcsrkxb.sHtML

[R08] 数值比较
来源：http://www.blog.fehbvm.com/Article/details/gvgbxizhu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.hesvh.cn/Article/details/gnngpwhhm.sHtML

[R09] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/glcnqchpa.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fehbvm.com/Article/details/gwhiqipyv.sHtML

[R10] 正则匹配
来源：http://blog.fehbvm.com/Article/details/gmxsuhldw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fehbvm.com/Article/details/goafxpiwn.sHtML

[R11] case 多分支
来源：http://read.share.hesvh.cn/Article/details/gzabifkzf.sHtML

case "$1" in
来源：http://www.share.hesvh.cn/Article/details/gbkvnumyp.sHtML

start) echo "启动" ;;
来源：http://mobile.zdbjq.cn/Article/details/grxgpohnc.sHtML

stop)  echo "停止" ;;
来源：http://mobile.hesvh.cn/Article/details/gghtwdssk.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fehbvm.com/Article/details/gxydlnzoc.sHtML

esac
来源：http://mobile.hesvh.cn/Article/details/gvwuosblq.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/gcghxtemj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/ggaamkjvo.sHtML

[R13] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/gzmzzzbpu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/glzsltdlv.sHtML

[R14] C 风格 for
来源：http://blog.hesvh.cn/Article/details/gitqfspfu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gzcbgcpvy.sHtML

[R15] while 逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gvrepxezb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.hesvh.cn/Article/details/gpxrtssez.sHtML

[R16] until 等待条件
来源：http://baike.zdbjq.cn/Article/details/gpovynuex.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gfasiatlp.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/gtxfmclcq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fehbvm.com/Article/details/gtvrdayxf.sHtML

[R18] 遍历数组
来源：http://blog.hesvh.cn/Article/details/gycxxgmyf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fehbvm.com/Article/details/gzejucgdv.sHtML

[R19] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gturgxkbh.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/gvsoudwjm.sHtML

[R20] 关联数组（字典）
来源：http://mobile.zdbjq.cn/Article/details/glwwgqyan.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.hesvh.cn/Article/details/gcuuvddka.sHtML

[R21] 字符串长度
来源：http://baike.fehbvm.com/Article/details/gpcoqkngo.sHtML

echo "${#s}"
来源：http://3g.hesvh.cn/Article/details/gszzlhlkd.sHtML

[R22] 截取子串
来源：http://wap.hesvh.cn/Article/details/gulpcdogv.sHtML

echo "${s:0:5}"
来源：http://mobile.fehbvm.com/Article/details/gmnyplzni.sHtML

[R23] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gdpwethwq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.hesvh.cn/Article/details/gagbcgqxb.sHtML

[R24] 大小写转换
来源：http://baike.fehbvm.com/Article/details/girxzufxn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.zdbjq.cn/Article/details/gxkalftfc.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.hesvh.cn/Article/details/gswdewngl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.zdbjq.cn/Article/details/gvixoadwm.sHtML

[R26] 命令替换
来源：http://mobile.zdbjq.cn/Article/details/gsqvwqoul.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.zdbjq.cn/Article/details/grewcjdhm.sHtML

[R27] 算术展开
来源：http://www.share.hesvh.cn/Article/details/gqgqogxwt.sHtML

echo $((1 + 2 * 3))
来源：http://3g.zdbjq.cn/Article/details/gktouegtj.sHtML

[R28] 浮点运算
来源：http://3g.zdbjq.cn/Article/details/gsfrlalhe.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.hesvh.cn/Article/details/ghlqbobii.sHtML

[R29] 定义函数
来源：http://www.share.fehbvm.com/Article/details/gpixjwxoo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fehbvm.com/Article/details/gltgrleoa.sHtML

[R30] 函数返回状态码
来源：http://3g.fehbvm.com/Article/details/gwavqytxr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/gvjmstpty.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/grepdabjx.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.zdbjq.cn/Article/details/gsasskkjg.sHtML

[R32] 参数个数校验
来源：http://wap.fehbvm.com/Article/details/gxacxmchb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/ghxgptjbr.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.hesvh.cn/Article/details/gkjnjkhzq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.zdbjq.cn/Article/details/gswcylevt.sHtML

[R34] 退出时清理
来源：http://3g.hesvh.cn/Article/details/gfgsmuwhi.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gtqbhfgkv.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/glijgqsik.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/gvzoumorn.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fehbvm.com/Article/details/guwkmmlyo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/gdbgqbrqq.sHtML

[R37] 把输出赋给变量
来源：http://read.share.hesvh.cn/Article/details/gddadqshx.sHtML

files=$(ls -1)
来源：http://baike.zdbjq.cn/Article/details/ghxkjjtfp.sHtML

[R38] 管道串联
来源：http://www.blog.zdbjq.cn/Article/details/gbjimzdck.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fehbvm.com/Article/details/gtcavgyid.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/gkernkcyz.sHtML

cmd > out.log 2>&1
来源：http://www.blog.hesvh.cn/Article/details/guilhzokd.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/gujudxgsx.sHtML

echo "log" >> out.log
来源：http://www.blog.fehbvm.com/Article/details/gujyzdqmb.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/gmjcguopc.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gdgmoirsa.sHtML

[R42] 输入重定向
来源：http://mobile.zdbjq.cn/Article/details/gbitpntgq.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/gorskwvmv.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fehbvm.com/Article/details/gznnohtxy.sHtML

find . -name "*.log" -type f
来源：http://www.share.zdbjq.cn/Article/details/glmkbkaeg.sHtML

[R44] 按修改时间查找
来源：http://read.share.fehbvm.com/Article/details/gucbqjsta.sHtML

find . -mtime -7 -type f
来源：http://wap.hesvh.cn/Article/details/gkmbynpex.sHtML

[R45] 批量删除
来源：http://m.share.hesvh.cn/Article/details/ggtwlixtf.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/gqapaonuq.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.hesvh.cn/Article/details/gjtkpiazi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gjdyvnusr.sHtML

[R47] sed 单行替换
来源：http://read.share.zdbjq.cn/Article/details/gkxyvlcxs.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fehbvm.com/Article/details/gkdrgqbli.sHtML

[R48] awk 取指定列
来源：http://www.share.zdbjq.cn/Article/details/grebcuapq.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gxqaxeybp.sHtML

[R49] awk 带条件
来源：http://wap.hesvh.cn/Article/details/gdzazdxkp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.zdbjq.cn/Article/details/gouxhjrge.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/gaffmfsfn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gjyyfympa.sHtML

[R51] 排序去重取前几
来源：http://mobile.hesvh.cn/Article/details/gklybqebn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fehbvm.com/Article/details/grpdtuiky.sHtML

[R52] 统计行数
来源：http://blog.zdbjq.cn/Article/details/gwfizovst.sHtML

wc -l a.txt
来源：http://www.share.zdbjq.cn/Article/details/grylibeco.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.hesvh.cn/Article/details/gftsjuuhc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.zdbjq.cn/Article/details/gqxetiabc.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/gtggxucza.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/gslmsoxpm.sHtML

[R55] 压缩与解压
来源：http://read.share.hesvh.cn/Article/details/gmdppihht.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fehbvm.com/Article/details/gtaoqiivk.sHtML

[R56] 远程拷贝
来源：http://wap.zdbjq.cn/Article/details/glztrejtw.sHtML

scp file user@host:/path/
来源：http://www.m.share.zdbjq.cn/Article/details/gwjkqrxne.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/gjpqhslbe.sHtML

ssh user@host 'uptime'
来源：http://baike.fehbvm.com/Article/details/gplufvxzp.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/ghswpsqpj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/giwpxcnzj.sHtML

[R59] 发 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gfnywpftx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fehbvm.com/Article/details/gtfbvftyu.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gihzsrfek.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/ggindehji.sHtML

[R61] 磁盘占用
来源：http://blog.fehbvm.com/Article/details/gdgtoqdhw.sHtML

df -h;  du -sh *
来源：http://www.share.fehbvm.com/Article/details/gsynmmyli.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/giyadvfdp.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fehbvm.com/Article/details/gfdwtdyto.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/gbvqnlgqp.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fehbvm.com/Article/details/grfsvbotw.sHtML

[R64] 结束进程
来源：http://read.share.fehbvm.com/Article/details/grwgtgbje.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/gndoufqvj.sHtML

[R65] 查看端口占用
来源：http://www.share.fehbvm.com/Article/details/gtwogjivk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fehbvm.com/Article/details/gcqcxlgqo.sHtML

[R66] 定时任务
来源：http://blog.hesvh.cn/Article/details/gtbqnatxe.sHtML

crontab -e;  crontab -l
来源：http://blog.zdbjq.cn/Article/details/gaxflipyn.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.zdbjq.cn/Article/details/gsymwveop.sHtML

openssl rand -hex 16
来源：http://blog.zdbjq.cn/Article/details/gurbhjmfa.sHtML

[R68] 计算文件校验值
来源：http://3g.hesvh.cn/Article/details/ggszidkmy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.hesvh.cn/Article/details/gueuhikuq.sHtML

[R69] 生成随机密码
来源：http://blog.zdbjq.cn/Article/details/gdsnlwqfe.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.zdbjq.cn/Article/details/gtwxcxodp.sHtML

[R70] 时间戳与互转
来源：http://www.blog.hesvh.cn/Article/details/gmuxhlrjx.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.hesvh.cn/Article/details/gfaoqfbsp.sHtML

[R71] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gjayooakh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.zdbjq.cn/Article/details/ggsboneuw.sHtML

[R72] 等待端口就绪
来源：http://baike.hesvh.cn/Article/details/gghfnnlzh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/giomwhtcn.sHtML

[R73] 分割大日志
来源：http://baike.zdbjq.cn/Article/details/gzdblbjvv.sHtML

split -l 1000 big.log part_
来源：http://mobile.zdbjq.cn/Article/details/gsrozucps.sHtML

[R74] 批量重命名
来源：http://3g.zdbjq.cn/Article/details/gehsxxali.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/goverujhh.sHtML

[R75] 导出环境变量
来源：http://blog.zdbjq.cn/Article/details/gnivdgawc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.hesvh.cn/Article/details/gultvlogg.sHtML

[R76] 使用临时文件
来源：http://www.blog.zdbjq.cn/Article/details/gjnvigbok.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gbbnmzwpp.sHtML

[R77] 读取用户输入
来源：http://www.share.fehbvm.com/Article/details/giloywbvs.sHtML

read -rp "请输入: " ans
来源：http://mobile.fehbvm.com/Article/details/giuthpjrt.sHtML

[R78] 交互式菜单
来源：http://baike.hesvh.cn/Article/details/gzurdlzqz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fehbvm.com/Article/details/gjdguhgsj.sHtML

[R79] 解析命令行选项
来源：http://wap.hesvh.cn/Article/details/gsktkrrca.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.hesvh.cn/Article/details/gkvjzklds.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/gwmzecnbq.sHtML

time ./run.sh
来源：http://read.share.hesvh.cn/Article/details/glvvutlkt.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjdvyehfc.sHtML

S. C / C++ 专题
来源：http://www.share.hesvh.cn/Article/details/gdvkrfjag.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdeicqnem.sHtML

[S01] C：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gaybjjsfh.sHtML

#include <stdio.h>
来源：http://read.share.fehbvm.com/Article/details/gjnihmrls.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.zdbjq.cn/Article/details/ghporvrai.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.zdbjq.cn/Article/details/gpvojlxhl.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.hesvh.cn/Article/details/gxwnjdsjt.sHtML

[S03] C：读入整数
来源：http://www.blog.zdbjq.cn/Article/details/geesqarom.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fehbvm.com/Article/details/gqwgayutf.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/ggoqivofv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.hesvh.cn/Article/details/gjwwyxeiv.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/gtisekamu.sHtML

strlen(s)
来源：http://www.share.hesvh.cn/Article/details/gbzlbiisi.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/gogsrlsht.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/gltqdlveu.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/gqbizciqr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/guuuhjwqc.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/gcqjrwidu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fehbvm.com/Article/details/gzysfsdqo.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fehbvm.com/Article/details/greotkgrm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.zdbjq.cn/Article/details/gcgavgpch.sHtML

[S10] C：指针与解引用
来源：http://3g.zdbjq.cn/Article/details/gepwvuxca.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fehbvm.com/Article/details/gheiyyris.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gkbajvtok.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.zdbjq.cn/Article/details/gduccrofl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fehbvm.com/Article/details/gerumwvxu.sHtML

fclose(f);
来源：http://wap.hesvh.cn/Article/details/gctlxnayc.sHtML

[S12] C：写文件
来源：http://mobile.fehbvm.com/Article/details/ggcpcusqr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/ghzzlspec.sHtML

[S13] C：宏定义
来源：http://blog.hesvh.cn/Article/details/gneqowvnx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/giwvkclks.sHtML

[S14] C：枚举
来源：http://www.m.share.hesvh.cn/Article/details/ganvucpdp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.zdbjq.cn/Article/details/gkpgrssgl.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/gxljopokp.sHtML

(double) a / b
来源：http://www.share.zdbjq.cn/Article/details/gertxijhq.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/grppetvra.sHtML

x |= (1 << 3);
来源：http://www.blog.zdbjq.cn/Article/details/gpkluiftt.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.hesvh.cn/Article/details/grwbcpvte.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/gvwcowdkf.sHtML

[S18] C：命令行参数
来源：http://read.share.fehbvm.com/Article/details/glpacbqtd.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/gnwbbkdva.sHtML

[S19] C：快速排序
来源：http://3g.zdbjq.cn/Article/details/gqtudoznr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gnoeyhvet.sHtML

[S20] C：二分查找
来源：http://wap.fehbvm.com/Article/details/ghqqusxkq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gamhawssg.sHtML

[S21] C：字符类别判断
来源：http://www.share.zdbjq.cn/Article/details/gitnwajkt.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fehbvm.com/Article/details/gxcehacts.sHtML

[S22] C：字符串转数字
来源：http://blog.hesvh.cn/Article/details/gsymlyeow.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/gjkfcrrro.sHtML

[S23] C：随机数
来源：http://www.blog.fehbvm.com/Article/details/gcgpprqho.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/gkokncklq.sHtML

[S24] C：获取本地时间
来源：http://www.share.hesvh.cn/Article/details/gystyxfzk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/gtkbeilsb.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gkagehguo.sHtML

memcpy(dst, src, n);
来源：http://www.share.fehbvm.com/Article/details/gipninpgt.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/gkaigqfun.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/gtedmtzdc.sHtML

[S27] C：定义常量
来源：http://baike.fehbvm.com/Article/details/gjpofivwy.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gtbcwbhmp.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/gdaqxbhwd.sHtML

static int counter = 0;
来源：http://3g.zdbjq.cn/Article/details/grajbauwz.sHtML

[S29] C：变参函数
来源：http://blog.hesvh.cn/Article/details/gqktxkoyc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fehbvm.com/Article/details/gihgrhrmv.sHtML

[S30] C：头文件保护
来源：http://baike.zdbjq.cn/Article/details/gxpvfbhzd.sHtML

#ifndef X_H
来源：http://www.m.share.zdbjq.cn/Article/details/geuumrqgu.sHtML

#define X_H
来源：http://m.share.zdbjq.cn/Article/details/gtsbompnp.sHtML

#endif
来源：http://www.blog.zdbjq.cn/Article/details/gliuepgsu.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/gusmgmlfz.sHtML

#include <iostream>
来源：http://blog.zdbjq.cn/Article/details/gjdellzof.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.zdbjq.cn/Article/details/ggetikgkw.sHtML

[S32] C++：字符串
来源：http://mobile.zdbjq.cn/Article/details/gjckoanzq.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fehbvm.com/Article/details/gudivyxcy.sHtML

[S33] C++：vector 增删
来源：http://www.share.fehbvm.com/Article/details/gwumzfncb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.zdbjq.cn/Article/details/gedajprxq.sHtML

[S34] C++：遍历 vector
来源：http://3g.fehbvm.com/Article/details/gaauchcox.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.zdbjq.cn/Article/details/gowiiyihq.sHtML

[S35] C++：map
来源：http://wap.fehbvm.com/Article/details/gzagnhqfn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gusdzzeul.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/gzdgmqkdd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gcvrwlhma.sHtML

[S37] C++：set
来源：http://m.share.hesvh.cn/Article/details/guigxljzb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gqzxeoovg.sHtML

[S38] C++：排序
来源：http://www.blog.fehbvm.com/Article/details/gvyqscwxs.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.hesvh.cn/Article/details/gkfcjkueo.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/gwwzazobl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/gxjrjmobl.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/gdfcbxoul.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.zdbjq.cn/Article/details/gazhspneb.sHtML

[S41] C++：类与构造函数
来源：http://3g.fehbvm.com/Article/details/gooyueokt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/gkjihudar.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fehbvm.com/Article/details/glmykceam.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.zdbjq.cn/Article/details/gckogmdlf.sHtML

[S43] C++：智能指针
来源：http://blog.hesvh.cn/Article/details/gpsgodoyb.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.zdbjq.cn/Article/details/ghkdrgjlr.sHtML

[S44] C++：引用传参
来源：http://mobile.fehbvm.com/Article/details/glrwfovbp.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/gyrelvvth.sHtML


<!-- 参考信息 -->