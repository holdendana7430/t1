代发 wailian999

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/gsngbcdgq.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/gkvdbvntm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.hesvh.cn/Article/details/gzcgubprb.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fehbvm.com/Article/details/gbngwneiy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fehbvm.com/Article/details/gozphwicj.sHtML

[Q75] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gsqsbxkpr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fehbvm.com/Article/details/gpqmfrsgy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/gnkdztrwj.sHtML

[Q76] 按天统计
来源：http://www.share.hesvh.cn/Article/details/ghbmuovkh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fehbvm.com/Article/details/gxodnxpdh.sHtML

[Q77] 时间加减
来源：http://mobile.hesvh.cn/Article/details/geskfqmae.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.hesvh.cn/Article/details/gfkzwldpz.sHtML

[Q78] 当前时间
来源：http://baike.zdbjq.cn/Article/details/gcgdiyryd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fehbvm.com/Article/details/gxiimyrcl.sHtML

[Q79] 字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gynllqhmc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fehbvm.com/Article/details/gbplhipwi.sHtML

[Q80] 字符串截取
来源：http://mobile.zdbjq.cn/Article/details/gtynbbpua.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/glmktydpw.sHtML

[Q81] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gxekylwme.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fehbvm.com/Article/details/gaaycxygp.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.hesvh.cn/Article/details/gycjdfhhh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gxcylrhst.sHtML

[Q83] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/grcylygkc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gwxbqzqvg.sHtML

[Q84] 去除首尾空格
来源：http://blog.fehbvm.com/Article/details/ggetqmrbe.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gvzmsdylp.sHtML

[Q85] 数值取整
来源：http://wap.zdbjq.cn/Article/details/gmnvfrggo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.zdbjq.cn/Article/details/gmkfkcpst.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/gytickpnz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.hesvh.cn/Article/details/ghskphhxf.sHtML

[Q87] JSON 字段做条件
来源：http://wap.hesvh.cn/Article/details/gfqrodkho.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.hesvh.cn/Article/details/gzyneuxsw.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.zdbjq.cn/Article/details/gaqadfxdf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.zdbjq.cn/Article/details/gqyzrsmgu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.zdbjq.cn/Article/details/ghdcvftmi.sHtML

[Q89] 判断表是否存在
来源：http://mobile.hesvh.cn/Article/details/grssjinil.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.zdbjq.cn/Article/details/gpgbdmwsa.sHtML

[Q90] 生成序号列
来源：http://m.share.fehbvm.com/Article/details/gjwyabvml.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.zdbjq.cn/Article/details/gdklsdhct.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqyzvaebr.sHtML

R. Bash 专题
来源：http://www.blog.zdbjq.cn/Article/details/gniuhsxgy.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gotqybjve.sHtML

[R01] shebang 与严格模式
来源：http://3g.zdbjq.cn/Article/details/golimpowl.sHtML

#!/usr/bin/env bash
来源：http://mobile.zdbjq.cn/Article/details/gikfwwrkk.sHtML

set -euo pipefail
来源：http://wap.zdbjq.cn/Article/details/gvdhdamxo.sHtML

[R02] 变量赋值与使用
来源：http://baike.fehbvm.com/Article/details/gowbmfdhh.sHtML

name="Tom"; echo "$name"
来源：http://3g.zdbjq.cn/Article/details/gkprsjyhj.sHtML

[R03] 只读变量
来源：http://blog.hesvh.cn/Article/details/gdbqktvju.sHtML

readonly PI=3.14
来源：http://wap.fehbvm.com/Article/details/gdwwfgmup.sHtML

[R04] 位置参数
来源：http://m.share.hesvh.cn/Article/details/ggzjrcbjx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fehbvm.com/Article/details/ggarutzig.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/gjuasuxno.sHtML

name="${1:-default}"
来源：http://3g.hesvh.cn/Article/details/gilztzrkw.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fehbvm.com/Article/details/gswjvpuil.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/goozunhqs.sHtML

[R07] if 判断文件
来源：http://www.m.share.fehbvm.com/Article/details/ghlfxwtom.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.zdbjq.cn/Article/details/gghmuocuw.sHtML

[R08] 数值比较
来源：http://www.blog.hesvh.cn/Article/details/glezufwda.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fehbvm.com/Article/details/ghelzpwdb.sHtML

[R09] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/glxjgltkx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.zdbjq.cn/Article/details/gehoedqro.sHtML

[R10] 正则匹配
来源：http://www.m.share.fehbvm.com/Article/details/gasosqmdn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fehbvm.com/Article/details/gfxyyeyoe.sHtML

[R11] case 多分支
来源：http://read.share.hesvh.cn/Article/details/gvlpcfrgl.sHtML

case "$1" in
来源：http://read.share.hesvh.cn/Article/details/gggjzvgjf.sHtML

start) echo "启动" ;;
来源：http://3g.hesvh.cn/Article/details/giqdbxojv.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/gpjayjmvw.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gwykjzqyg.sHtML

esac
来源：http://blog.hesvh.cn/Article/details/ggdxognoz.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/genibwkwm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.zdbjq.cn/Article/details/gftsegoix.sHtML

[R13] for 计数循环
来源：http://m.share.fehbvm.com/Article/details/gevhuvnjx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gkjmpxxtw.sHtML

[R14] C 风格 for
来源：http://www.blog.hesvh.cn/Article/details/gqlspmkym.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gqupdvqoh.sHtML

[R15] while 逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gecuvtuzu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fehbvm.com/Article/details/greapwypb.sHtML

[R16] until 等待条件
来源：http://read.share.hesvh.cn/Article/details/grbszbezj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gqyvpexio.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/gesgjbcdq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fehbvm.com/Article/details/gcadbkinn.sHtML

[R18] 遍历数组
来源：http://wap.hesvh.cn/Article/details/glpncrgqd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.zdbjq.cn/Article/details/gjevpqvor.sHtML

[R19] 数组长度
来源：http://wap.fehbvm.com/Article/details/gopxvokzz.sHtML

echo "${#arr[@]}"
来源：http://blog.hesvh.cn/Article/details/giemkffrv.sHtML

[R20] 关联数组（字典）
来源：http://m.share.zdbjq.cn/Article/details/gnbeanoff.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fehbvm.com/Article/details/grfnoskow.sHtML

[R21] 字符串长度
来源：http://3g.fehbvm.com/Article/details/gpywpdkan.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/gveamipdw.sHtML

[R22] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gzefuoxem.sHtML

echo "${s:0:5}"
来源：http://www.blog.fehbvm.com/Article/details/glvxfbuok.sHtML

[R23] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gzwkhdzve.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.hesvh.cn/Article/details/gcjzkbowl.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gnurzqnwn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.zdbjq.cn/Article/details/gtdcybhns.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.zdbjq.cn/Article/details/golwqbddl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.zdbjq.cn/Article/details/gvfqjmlmy.sHtML

[R26] 命令替换
来源：http://wap.zdbjq.cn/Article/details/grbvfisaf.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.hesvh.cn/Article/details/gyvgzgcwt.sHtML

[R27] 算术展开
来源：http://www.blog.fehbvm.com/Article/details/guknlmvke.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.hesvh.cn/Article/details/ghatmsuhk.sHtML

[R28] 浮点运算
来源：http://www.m.share.hesvh.cn/Article/details/gzpfovjia.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fehbvm.com/Article/details/gwknvxmmc.sHtML

[R29] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gpnemytce.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/gkntfstty.sHtML

[R30] 函数返回状态码
来源：http://www.share.zdbjq.cn/Article/details/gfpumcaqd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fehbvm.com/Article/details/glcpyopii.sHtML

[R31] 局部变量
来源：http://wap.fehbvm.com/Article/details/gprcxnzxv.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.hesvh.cn/Article/details/gdnonumhh.sHtML

[R32] 参数个数校验
来源：http://baike.fehbvm.com/Article/details/glhaolsvu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/ghmekdocb.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.zdbjq.cn/Article/details/guvxjuaqp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fehbvm.com/Article/details/gacktgujr.sHtML

[R34] 退出时清理
来源：http://www.m.share.hesvh.cn/Article/details/ggyoxgaqd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gtvgieznn.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/gdsjstxwf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fehbvm.com/Article/details/gxsgqeohm.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fehbvm.com/Article/details/gtpqpkway.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fehbvm.com/Article/details/gacnopqhv.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.zdbjq.cn/Article/details/gvesprtkf.sHtML

files=$(ls -1)
来源：http://read.share.fehbvm.com/Article/details/gffwnmoea.sHtML

[R38] 管道串联
来源：http://read.share.fehbvm.com/Article/details/gaeodmzws.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.zdbjq.cn/Article/details/gevjeojyq.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.hesvh.cn/Article/details/gcsqmqlft.sHtML

cmd > out.log 2>&1
来源：http://wap.fehbvm.com/Article/details/gzpunmrwx.sHtML

[R40] 追加写日志
来源：http://www.blog.hesvh.cn/Article/details/gujigzfwf.sHtML

echo "log" >> out.log
来源：http://baike.fehbvm.com/Article/details/gkyfpvpav.sHtML

[R41] 丢弃输出
来源：http://wap.fehbvm.com/Article/details/ghxhflook.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gokdzuerq.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/ghvrbwajk.sHtML

wc -l < a.txt
来源：http://www.share.zdbjq.cn/Article/details/gtypthvbh.sHtML

[R43] 按名字查找文件
来源：http://baike.zdbjq.cn/Article/details/gzfmfckpd.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/gwydtxruc.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fehbvm.com/Article/details/glwbmtpyq.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/gqoviisgu.sHtML

[R45] 批量删除
来源：http://www.m.share.zdbjq.cn/Article/details/gijdpifmy.sHtML

find . -name "*.tmp" -delete
来源：http://baike.hesvh.cn/Article/details/grnpkfiwt.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fehbvm.com/Article/details/gjjvcbffl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/gognnmlre.sHtML

[R47] sed 单行替换
来源：http://read.share.hesvh.cn/Article/details/gpqsprfqd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.hesvh.cn/Article/details/gtklkfzxd.sHtML

[R48] awk 取指定列
来源：http://blog.zdbjq.cn/Article/details/gbzrstwjf.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gnlclztbg.sHtML

[R49] awk 带条件
来源：http://m.share.hesvh.cn/Article/details/gaaclmusp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.hesvh.cn/Article/details/grdydcjzo.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/grfxvufnc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fehbvm.com/Article/details/ggmwbtnrg.sHtML

[R51] 排序去重取前几
来源：http://m.share.fehbvm.com/Article/details/gwfoxhqgm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fehbvm.com/Article/details/gphgptfgj.sHtML

[R52] 统计行数
来源：http://read.share.fehbvm.com/Article/details/glddhqtnu.sHtML

wc -l a.txt
来源：http://m.share.zdbjq.cn/Article/details/giniqjudu.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/gpowvgsnc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/gdwizlffl.sHtML

[R54] 比较两个文件
来源：http://www.m.share.hesvh.cn/Article/details/gezyvyjvq.sHtML

diff a.txt b.txt
来源：http://blog.zdbjq.cn/Article/details/gwcjwvmjq.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/grdordtmz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.hesvh.cn/Article/details/gluikhgxc.sHtML

[R56] 远程拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gesoysbtr.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/gruyflsoo.sHtML

[R57] 远程执行命令
来源：http://blog.hesvh.cn/Article/details/gmtkcdaga.sHtML

ssh user@host 'uptime'
来源：http://read.share.fehbvm.com/Article/details/gbiipzxpk.sHtML

[R58] 下载文件
来源：http://www.share.fehbvm.com/Article/details/gikhgzhbk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.hesvh.cn/Article/details/gbvnfavae.sHtML

[R59] 发 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gwheildwx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fehbvm.com/Article/details/gifbksujp.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gnxpdevhn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.hesvh.cn/Article/details/gqrvqoqfi.sHtML

[R61] 磁盘占用
来源：http://wap.zdbjq.cn/Article/details/grabwzvzo.sHtML

df -h;  du -sh *
来源：http://wap.fehbvm.com/Article/details/gsesoqdbc.sHtML

[R62] 找最占空间的文件
来源：http://read.share.hesvh.cn/Article/details/gxcfipvku.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/gcxgnvfmt.sHtML

[R63] 内存与进程
来源：http://blog.hesvh.cn/Article/details/gbvlaskxk.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fehbvm.com/Article/details/giahugxqg.sHtML

[R64] 结束进程
来源：http://www.share.hesvh.cn/Article/details/gqzorrcqk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.zdbjq.cn/Article/details/gqpaqmuvy.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/grelleono.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/gbnvisesj.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/gcwtducep.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/gjlxinamv.sHtML

[R67] 生成随机十六进制串
来源：http://baike.zdbjq.cn/Article/details/gigvxtvgz.sHtML

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/gtxsxzdab.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/grkqaxlqj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fehbvm.com/Article/details/gpngwqqpy.sHtML

[R69] 生成随机密码
来源：http://blog.hesvh.cn/Article/details/gfifebcez.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fehbvm.com/Article/details/gpivatnoq.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.zdbjq.cn/Article/details/geqcnsmiu.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fehbvm.com/Article/details/gtgzxexxb.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gmfyxquzp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.hesvh.cn/Article/details/gezmhurdg.sHtML

[R72] 等待端口就绪
来源：http://mobile.hesvh.cn/Article/details/grzzsdnby.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gshsjmkyw.sHtML

[R73] 分割大日志
来源：http://baike.fehbvm.com/Article/details/gsiycnyzi.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/gwddlqzmo.sHtML

[R74] 批量重命名
来源：http://m.share.fehbvm.com/Article/details/gprybprvu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/grgxurpcw.sHtML

[R75] 导出环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gbfngpsmb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/gyxclezrq.sHtML

[R76] 使用临时文件
来源：http://3g.hesvh.cn/Article/details/gsvnzgbrw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gaddjxbrn.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/gdegwgzhx.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fehbvm.com/Article/details/gsmyewmpv.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/grqinuxui.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/gjtsqimjr.sHtML

[R79] 解析命令行选项
来源：http://blog.fehbvm.com/Article/details/gumlgfkaj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fehbvm.com/Article/details/gmmxgfnvg.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.zdbjq.cn/Article/details/gzrkdtwkd.sHtML

time ./run.sh
来源：http://wap.hesvh.cn/Article/details/gpcihggpp.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpfrnxtst.sHtML

S. C / C++ 专题
来源：http://www.m.share.hesvh.cn/Article/details/gezqmqekz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gyyhpsomr.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/gzujncfvo.sHtML

#include <stdio.h>
来源：http://www.blog.fehbvm.com/Article/details/gtxtduxty.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fehbvm.com/Article/details/guhtotwcc.sHtML

[S02] C：变量与格式化输出
来源：http://3g.hesvh.cn/Article/details/ggleyatxl.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/gxprepuvb.sHtML

[S03] C：读入整数
来源：http://3g.fehbvm.com/Article/details/gziyfthay.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.hesvh.cn/Article/details/geivgsdjc.sHtML

[S04] C：字符串复制
来源：http://3g.hesvh.cn/Article/details/gckghogvg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.zdbjq.cn/Article/details/gbkkewyhe.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gfonwimqd.sHtML

strlen(s)
来源：http://www.blog.fehbvm.com/Article/details/ggjwwhhuz.sHtML

[S06] C：字符串比较
来源：http://3g.zdbjq.cn/Article/details/gqtlrelmx.sHtML

strcmp(a, b) == 0
来源：http://wap.zdbjq.cn/Article/details/gbiqizven.sHtML

[S07] C：数组遍历求和
来源：http://3g.hesvh.cn/Article/details/gliknnlio.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fehbvm.com/Article/details/gtewnemsc.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.zdbjq.cn/Article/details/gpqgkrxhg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.zdbjq.cn/Article/details/gwuqdmqdp.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/gotinfjhg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.zdbjq.cn/Article/details/gczhykace.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/gugltyjeb.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/gvleyalnn.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gfxutkjwu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.zdbjq.cn/Article/details/gdsayzgxi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fehbvm.com/Article/details/gdxzfpwze.sHtML

fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gobnghxpu.sHtML

[S12] C：写文件
来源：http://wap.zdbjq.cn/Article/details/gryguyrvm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gnstyfjvi.sHtML

[S13] C：宏定义
来源：http://baike.zdbjq.cn/Article/details/gdmozdpmk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fehbvm.com/Article/details/geksylatc.sHtML

[S14] C：枚举
来源：http://mobile.zdbjq.cn/Article/details/gsflmifwc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.zdbjq.cn/Article/details/gmrfztfjr.sHtML

[S15] C：类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gnojbidne.sHtML

(double) a / b
来源：http://blog.zdbjq.cn/Article/details/gpjqwscwb.sHtML

[S16] C：位操作置位
来源：http://baike.hesvh.cn/Article/details/gtgreqizd.sHtML

x |= (1 << 3);
来源：http://baike.hesvh.cn/Article/details/gnwsavgdb.sHtML

[S17] C：安全拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gdpluhkhp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fehbvm.com/Article/details/gjrfifsdo.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/ggfgotaju.sHtML

int main(int argc, char **argv)
来源：http://blog.hesvh.cn/Article/details/goshsuhhm.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/gvqgjbbfn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gseihyxfx.sHtML

[S20] C：二分查找
来源：http://m.share.zdbjq.cn/Article/details/gbonlkevy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gzdqygohp.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/gjzcsyybf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.zdbjq.cn/Article/details/gheolpkeg.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gjvxulcmd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fehbvm.com/Article/details/gataoiczh.sHtML

[S23] C：随机数
来源：http://3g.fehbvm.com/Article/details/garxlsylm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/gmxiydgmf.sHtML

[S24] C：获取本地时间
来源：http://baike.zdbjq.cn/Article/details/gdciqqqnr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gmtkivbeu.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gxqjbxfzf.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/gdnpyuyvk.sHtML

[S26] C：内存清零
来源：http://www.share.hesvh.cn/Article/details/gmajiknbb.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fehbvm.com/Article/details/gbvpwhbvr.sHtML

[S27] C：定义常量
来源：http://wap.fehbvm.com/Article/details/gnezzghyv.sHtML

const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gldflpqab.sHtML

[S28] C：静态变量
来源：http://www.blog.fehbvm.com/Article/details/gbpaftpmb.sHtML

static int counter = 0;
来源：http://www.share.fehbvm.com/Article/details/gqmuzkhff.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/gwobaryfz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.hesvh.cn/Article/details/gplqagwvp.sHtML

[S30] C：头文件保护
来源：http://wap.zdbjq.cn/Article/details/ggincmkwm.sHtML

#ifndef X_H
来源：http://mobile.hesvh.cn/Article/details/gctkdfmos.sHtML

#define X_H
来源：http://baike.zdbjq.cn/Article/details/gjjwrjgnr.sHtML

#endif
来源：http://mobile.hesvh.cn/Article/details/gbsljmuvi.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/gxjzvegnd.sHtML

#include <iostream>
来源：http://baike.hesvh.cn/Article/details/gljtvvshn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/gbgzzizxg.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/ggabkumwo.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.zdbjq.cn/Article/details/gqktnwzee.sHtML

[S33] C++：vector 增删
来源：http://m.share.zdbjq.cn/Article/details/gjojifmja.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.zdbjq.cn/Article/details/gqvofburi.sHtML

[S34] C++：遍历 vector
来源：http://www.share.hesvh.cn/Article/details/gbpgdtbqn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/gsrpwldxs.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/guvsnpicp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/guncrmvic.sHtML

[S36] C++：unordered_map
来源：http://blog.fehbvm.com/Article/details/gvgekbkys.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gwmssuyxx.sHtML

[S37] C++：set
来源：http://www.m.share.fehbvm.com/Article/details/gwaqbbyfr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/gtaplktgu.sHtML

[S38] C++：排序
来源：http://www.m.share.zdbjq.cn/Article/details/gbgwlrixn.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gtzopshue.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.zdbjq.cn/Article/details/gcxprnomd.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/gobonntmv.sHtML

[S40] C++：查找元素
来源：http://www.m.share.zdbjq.cn/Article/details/givnwzhyc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.hesvh.cn/Article/details/gfcmkgxrr.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fehbvm.com/Article/details/gfpscqtyo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/gvvxvmsqd.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/gftmqinlq.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.zdbjq.cn/Article/details/gbkvieuke.sHtML


<!-- 参考信息 -->