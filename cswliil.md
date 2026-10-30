代发 wailian999

ANALYZE TABLE users;
来源：http://www.blog.hesvh.cn/Article/details/gtbcpzusu.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.zdbjq.cn/Article/details/ghziysebn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.zdbjq.cn/Article/details/gedsfoxdg.sHtML

[Q72] 查看索引
来源：http://read.share.zdbjq.cn/Article/details/gtubecsqy.sHtML

SHOW INDEX FROM users;
来源：http://blog.zdbjq.cn/Article/details/gfzeetrbl.sHtML

[Q73] 查看表状态
来源：http://www.blog.hesvh.cn/Article/details/gjazydsvv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fehbvm.com/Article/details/gatenlyyk.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/guaqvxkvu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.hesvh.cn/Article/details/gpuoigoam.sHtML

[Q75] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gwpznkkrm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/glpohgvxz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fehbvm.com/Article/details/gpuwogxfq.sHtML

[Q76] 按天统计
来源：http://wap.hesvh.cn/Article/details/gxavnapxp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.hesvh.cn/Article/details/gnurfwjsr.sHtML

[Q77] 时间加减
来源：http://www.blog.hesvh.cn/Article/details/gxnnewcow.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fehbvm.com/Article/details/glignwuzx.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/gnmwawadv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fehbvm.com/Article/details/gzdxrjngk.sHtML

[Q79] 字符串拼接
来源：http://blog.zdbjq.cn/Article/details/gxkpkzfrh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/grtiudpkh.sHtML

[Q80] 字符串截取
来源：http://blog.hesvh.cn/Article/details/gmftcrhak.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/grhkqmyey.sHtML

[Q81] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/grcrujtcv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.zdbjq.cn/Article/details/guurrsjmf.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.hesvh.cn/Article/details/gdnsfnnyc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gmsgvwici.sHtML

[Q83] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gnfgvjmlo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gwsbylmsz.sHtML

[Q84] 去除首尾空格
来源：http://blog.fehbvm.com/Article/details/gupbpqzqr.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gwzlyeqyk.sHtML

[Q85] 数值取整
来源：http://read.share.fehbvm.com/Article/details/gfmhuvbtg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fehbvm.com/Article/details/glqfgcqnc.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.hesvh.cn/Article/details/gabdhsrxt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.zdbjq.cn/Article/details/goatcuqyh.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fehbvm.com/Article/details/givhrpkma.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.zdbjq.cn/Article/details/glzdlvulj.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.zdbjq.cn/Article/details/gsxsekxui.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fehbvm.com/Article/details/gnjdfykur.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.hesvh.cn/Article/details/gegugpdjl.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gdnftgztt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.zdbjq.cn/Article/details/gfhnsmcky.sHtML

[Q90] 生成序号列
来源：http://wap.hesvh.cn/Article/details/gejkicepq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fehbvm.com/Article/details/gkuirmynd.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gjdjjahrp.sHtML

R. Bash 专题
来源：http://mobile.zdbjq.cn/Article/details/gsaxiihus.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpabbahde.sHtML

[R01] shebang 与严格模式
来源：http://www.share.hesvh.cn/Article/details/gsczlxyam.sHtML

#!/usr/bin/env bash
来源：http://mobile.fehbvm.com/Article/details/gucyptgbc.sHtML

set -euo pipefail
来源：http://m.share.fehbvm.com/Article/details/gziecptrg.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fehbvm.com/Article/details/gvzwgpegw.sHtML

name="Tom"; echo "$name"
来源：http://m.share.hesvh.cn/Article/details/gbchylrau.sHtML

[R03] 只读变量
来源：http://www.blog.fehbvm.com/Article/details/gusbtjdcc.sHtML

readonly PI=3.14
来源：http://baike.fehbvm.com/Article/details/gdganhmpg.sHtML

[R04] 位置参数
来源：http://www.m.share.zdbjq.cn/Article/details/gxzrzfevw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fehbvm.com/Article/details/grdavyfyb.sHtML

[R05] 参数默认值
来源：http://mobile.zdbjq.cn/Article/details/givgvkiym.sHtML

name="${1:-default}"
来源：http://read.share.hesvh.cn/Article/details/gqmtbhakr.sHtML

[R06] 判断命令是否存在
来源：http://blog.hesvh.cn/Article/details/gjwkddwgy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/goannskju.sHtML

[R07] if 判断文件
来源：http://3g.zdbjq.cn/Article/details/gyujvexwn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fehbvm.com/Article/details/ghizkplbt.sHtML

[R08] 数值比较
来源：http://blog.hesvh.cn/Article/details/gyjzoskep.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.zdbjq.cn/Article/details/gvcqauzyi.sHtML

[R09] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/gohklgxiz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fehbvm.com/Article/details/gxddpbevk.sHtML

[R10] 正则匹配
来源：http://mobile.zdbjq.cn/Article/details/gnaptgowz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gttwxknaz.sHtML

[R11] case 多分支
来源：http://blog.hesvh.cn/Article/details/gfkkrlpoi.sHtML

case "$1" in
来源：http://read.share.fehbvm.com/Article/details/guqdddtor.sHtML

start) echo "启动" ;;
来源：http://read.share.hesvh.cn/Article/details/gqfaiyruj.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/glimgjkwt.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.hesvh.cn/Article/details/goalaoobf.sHtML

esac
来源：http://m.share.zdbjq.cn/Article/details/gbfaryfyd.sHtML

[R12] for 遍历文件
来源：http://mobile.fehbvm.com/Article/details/grbekuavy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/gwbhsgnxl.sHtML

[R13] for 计数循环
来源：http://wap.hesvh.cn/Article/details/ggiktpaaz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gzeptizyv.sHtML

[R14] C 风格 for
来源：http://www.blog.hesvh.cn/Article/details/gxxehtqxf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gfmhsgqpe.sHtML

[R15] while 逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gonoebkau.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fehbvm.com/Article/details/gmntkjbtv.sHtML

[R16] until 等待条件
来源：http://mobile.fehbvm.com/Article/details/gxuoqcnrk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gkzbywwte.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.zdbjq.cn/Article/details/gcjrtaaao.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fehbvm.com/Article/details/ggctpkupd.sHtML

[R18] 遍历数组
来源：http://3g.fehbvm.com/Article/details/gjhxpesmz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.hesvh.cn/Article/details/ghcbltwth.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gclofvykh.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fehbvm.com/Article/details/guuzmoejr.sHtML

[R20] 关联数组（字典）
来源：http://read.share.zdbjq.cn/Article/details/gfsbtsdil.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.zdbjq.cn/Article/details/gvtwfpxnn.sHtML

[R21] 字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gbbszihyq.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/gvhtaxndr.sHtML

[R22] 截取子串
来源：http://wap.fehbvm.com/Article/details/gdhkpodnb.sHtML

echo "${s:0:5}"
来源：http://3g.zdbjq.cn/Article/details/gigdilyui.sHtML

[R23] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gxncjtrbo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.hesvh.cn/Article/details/gbrrssesg.sHtML

[R24] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gdgxrawjw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.zdbjq.cn/Article/details/gmnpyvrnt.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.zdbjq.cn/Article/details/gibtnucet.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fehbvm.com/Article/details/gfsziumgn.sHtML

[R26] 命令替换
来源：http://wap.hesvh.cn/Article/details/gomgkehty.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.hesvh.cn/Article/details/gkakmjmah.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/gxcbnibha.sHtML

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/gaksmgaam.sHtML

[R28] 浮点运算
来源：http://3g.hesvh.cn/Article/details/gsyzevcxt.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.zdbjq.cn/Article/details/ggixvhlql.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gihuuhrwn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.zdbjq.cn/Article/details/gwrvwdwog.sHtML

[R30] 函数返回状态码
来源：http://read.share.zdbjq.cn/Article/details/gdmdcumww.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fehbvm.com/Article/details/gdsvlyfxa.sHtML

[R31] 局部变量
来源：http://baike.fehbvm.com/Article/details/gfnnjgreh.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.hesvh.cn/Article/details/giumfkaky.sHtML

[R32] 参数个数校验
来源：http://wap.zdbjq.cn/Article/details/gxkwrmkey.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gqmjkzucs.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/giceqdamh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.hesvh.cn/Article/details/ggaecmayu.sHtML

[R34] 退出时清理
来源：http://m.share.fehbvm.com/Article/details/gfarwrfvz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gadhefttf.sHtML

[R35] 后台执行并等待
来源：http://wap.zdbjq.cn/Article/details/glhseynsi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.hesvh.cn/Article/details/gnpcgfdyx.sHtML

[R36] 并发执行多个任务
来源：http://wap.hesvh.cn/Article/details/gphjqbatg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.hesvh.cn/Article/details/grsbiqnoc.sHtML

[R37] 把输出赋给变量
来源：http://m.share.zdbjq.cn/Article/details/gsrynswjt.sHtML

files=$(ls -1)
来源：http://www.blog.zdbjq.cn/Article/details/gbadzyliy.sHtML

[R38] 管道串联
来源：http://3g.zdbjq.cn/Article/details/gylcacuqp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/gkqlgczpl.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.hesvh.cn/Article/details/gtalrcvsn.sHtML

cmd > out.log 2>&1
来源：http://baike.fehbvm.com/Article/details/gqtuzwjni.sHtML

[R40] 追加写日志
来源：http://www.blog.fehbvm.com/Article/details/gxziegyyt.sHtML

echo "log" >> out.log
来源：http://baike.fehbvm.com/Article/details/gbvvtdgpj.sHtML

[R41] 丢弃输出
来源：http://www.share.fehbvm.com/Article/details/gqxgbnheu.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gttascdno.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/gankbhdij.sHtML

wc -l < a.txt
来源：http://www.share.zdbjq.cn/Article/details/gzwzakzfl.sHtML

[R43] 按名字查找文件
来源：http://m.share.zdbjq.cn/Article/details/gpgrocqjn.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/ghzowpydj.sHtML

[R44] 按修改时间查找
来源：http://read.share.zdbjq.cn/Article/details/gwtmymibd.sHtML

find . -mtime -7 -type f
来源：http://www.blog.hesvh.cn/Article/details/gvuvmbfoe.sHtML

[R45] 批量删除
来源：http://baike.fehbvm.com/Article/details/grqskvxjc.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.zdbjq.cn/Article/details/gqczxkwtu.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/gedwyvkei.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fehbvm.com/Article/details/gxqtsjtyu.sHtML

[R47] sed 单行替换
来源：http://www.m.share.hesvh.cn/Article/details/gkoyulogr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fehbvm.com/Article/details/gfxmektmf.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/genuvlfzm.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gevinqvub.sHtML

[R49] awk 带条件
来源：http://www.share.hesvh.cn/Article/details/gsevxigpd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/ghmsbnrsj.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/guwghvqva.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gvpmlvlpr.sHtML

[R51] 排序去重取前几
来源：http://m.share.hesvh.cn/Article/details/gsfnqwdbp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gdmjssbdk.sHtML

[R52] 统计行数
来源：http://www.share.hesvh.cn/Article/details/gnvyramlv.sHtML

wc -l a.txt
来源：http://3g.hesvh.cn/Article/details/gfmfiulqc.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/gebupdlyi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.zdbjq.cn/Article/details/gbeqwqyav.sHtML

[R54] 比较两个文件
来源：http://m.share.hesvh.cn/Article/details/gpasntshc.sHtML

diff a.txt b.txt
来源：http://wap.fehbvm.com/Article/details/gggylsafd.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/ggwaoatmf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.hesvh.cn/Article/details/ggtpxcixx.sHtML

[R56] 远程拷贝
来源：http://wap.zdbjq.cn/Article/details/ghmuuxace.sHtML

scp file user@host:/path/
来源：http://wap.hesvh.cn/Article/details/guzlzdron.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/gadgbpnys.sHtML

ssh user@host 'uptime'
来源：http://www.blog.zdbjq.cn/Article/details/ggzbdhzrr.sHtML

[R58] 下载文件
来源：http://mobile.hesvh.cn/Article/details/gmzcddppf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.hesvh.cn/Article/details/gccaikgjt.sHtML

[R59] 发 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gmmrfnuej.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fehbvm.com/Article/details/gjbzjdzrc.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/ggoxfwnre.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fehbvm.com/Article/details/gydrnokfe.sHtML

[R61] 磁盘占用
来源：http://m.share.hesvh.cn/Article/details/gvpvzsbzx.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/ggploqldo.sHtML

[R62] 找最占空间的文件
来源：http://mobile.hesvh.cn/Article/details/gefhxyiof.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.hesvh.cn/Article/details/gghjxdlpk.sHtML

[R63] 内存与进程
来源：http://www.m.share.zdbjq.cn/Article/details/gcoolkopv.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.zdbjq.cn/Article/details/gnbwasqpg.sHtML

[R64] 结束进程
来源：http://mobile.zdbjq.cn/Article/details/gigkomopb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/gzyxpiafu.sHtML

[R65] 查看端口占用
来源：http://m.share.hesvh.cn/Article/details/gvkgeokax.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.zdbjq.cn/Article/details/ghpianlwr.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/glocojrnx.sHtML

crontab -e;  crontab -l
来源：http://3g.zdbjq.cn/Article/details/gfoktxnuv.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.zdbjq.cn/Article/details/gbqozqiya.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/giygimuoz.sHtML

[R68] 计算文件校验值
来源：http://mobile.fehbvm.com/Article/details/gihwashyw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fehbvm.com/Article/details/gmzopcegn.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/ggutyduor.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fehbvm.com/Article/details/goghprxuu.sHtML

[R70] 时间戳与互转
来源：http://read.share.fehbvm.com/Article/details/gkrweilan.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/gykpxtpww.sHtML

[R71] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gtorecgbq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/ggnvctsva.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/gszprdqfi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gltuonpqe.sHtML

[R73] 分割大日志
来源：http://3g.zdbjq.cn/Article/details/gfzzdwdco.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/grpogugta.sHtML

[R74] 批量重命名
来源：http://www.share.hesvh.cn/Article/details/gazrbdgww.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fehbvm.com/Article/details/gypfccjbk.sHtML

[R75] 导出环境变量
来源：http://mobile.hesvh.cn/Article/details/ggjiqzkhh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fehbvm.com/Article/details/gmyeaaito.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/govtfazkw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gkhsteyzb.sHtML

[R77] 读取用户输入
来源：http://3g.zdbjq.cn/Article/details/gmxayynsy.sHtML

read -rp "请输入: " ans
来源：http://m.share.fehbvm.com/Article/details/gzcwxtxmx.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/gydaazjuz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fehbvm.com/Article/details/gfozqssxt.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/gxhzsrlzd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fehbvm.com/Article/details/gyhgzuilc.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.zdbjq.cn/Article/details/gnclsgpcx.sHtML

time ./run.sh
来源：http://baike.hesvh.cn/Article/details/ggokhgchm.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjoucxlfw.sHtML

S. C / C++ 专题
来源：http://read.share.fehbvm.com/Article/details/gahgtvykj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjqsoeymf.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/gxxjjrhjt.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/gtfhfqqqv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.zdbjq.cn/Article/details/gbuupiwxl.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/getarbnmb.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fehbvm.com/Article/details/gxvtagclq.sHtML

[S03] C：读入整数
来源：http://blog.hesvh.cn/Article/details/gvocssvoq.sHtML

int x; scanf("%d", &x);
来源：http://mobile.zdbjq.cn/Article/details/gmgwdnjsg.sHtML

[S04] C：字符串复制
来源：http://wap.zdbjq.cn/Article/details/ggpwlsrof.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fehbvm.com/Article/details/gmaisbewg.sHtML

[S05] C：字符串长度
来源：http://read.share.fehbvm.com/Article/details/gsyjzffvq.sHtML

strlen(s)
来源：http://mobile.hesvh.cn/Article/details/gaktxuzjm.sHtML

[S06] C：字符串比较
来源：http://m.share.hesvh.cn/Article/details/gexprcqjg.sHtML

strcmp(a, b) == 0
来源：http://www.share.zdbjq.cn/Article/details/gymigrucb.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/gtztktntc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.hesvh.cn/Article/details/guhbqxehy.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.hesvh.cn/Article/details/gxddwlnrs.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.hesvh.cn/Article/details/gfeheycws.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/gylvcwuku.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fehbvm.com/Article/details/gddpkgnpn.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/grvzaxfvp.sHtML

int *p = &a;  *p = 5;
来源：http://baike.hesvh.cn/Article/details/grbwzsrha.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/ghckdbabg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fehbvm.com/Article/details/grukhzkyx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gjxtxtqcp.sHtML

fclose(f);
来源：http://blog.hesvh.cn/Article/details/gbyajxtpv.sHtML

[S12] C：写文件
来源：http://wap.fehbvm.com/Article/details/gvlqaorim.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.hesvh.cn/Article/details/gqxbyrmjj.sHtML

[S13] C：宏定义
来源：http://mobile.zdbjq.cn/Article/details/gcsknmjzi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.hesvh.cn/Article/details/guczzmgqu.sHtML

[S14] C：枚举
来源：http://baike.zdbjq.cn/Article/details/grcphowqf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.hesvh.cn/Article/details/grxgllmlu.sHtML

[S15] C：类型转换
来源：http://mobile.hesvh.cn/Article/details/gtxnxxqoo.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/gmyfuxnzd.sHtML

[S16] C：位操作置位
来源：http://www.share.fehbvm.com/Article/details/graimyedv.sHtML

x |= (1 << 3);
来源：http://3g.hesvh.cn/Article/details/geqlqlymu.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fehbvm.com/Article/details/gfphjepew.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.hesvh.cn/Article/details/grjhowhnx.sHtML

[S18] C：命令行参数
来源：http://blog.zdbjq.cn/Article/details/gtoihyxsy.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.hesvh.cn/Article/details/gixylfizk.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/gxibdqzeh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gjhoojguk.sHtML

[S20] C：二分查找
来源：http://blog.zdbjq.cn/Article/details/gleodacqc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gxinwkzfz.sHtML

[S21] C：字符类别判断
来源：http://m.share.hesvh.cn/Article/details/gudzumunh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fehbvm.com/Article/details/gscbxitlc.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/gofwcbdoo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fehbvm.com/Article/details/gycnrgjub.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/gtbjccghe.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.hesvh.cn/Article/details/gczekyrqr.sHtML

[S24] C：获取本地时间
来源：http://read.share.fehbvm.com/Article/details/gdwamuoiz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.hesvh.cn/Article/details/gersfcocs.sHtML

[S25] C：内存拷贝
来源：http://www.blog.hesvh.cn/Article/details/giqojmkti.sHtML

memcpy(dst, src, n);
来源：http://m.share.zdbjq.cn/Article/details/ggaqoqwij.sHtML

[S26] C：内存清零
来源：http://wap.zdbjq.cn/Article/details/gisdxlqmv.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/gmuvpabhv.sHtML

[S27] C：定义常量
来源：http://wap.zdbjq.cn/Article/details/gdwpsklhf.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gxcdcedxx.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/gzhqyrbxl.sHtML

static int counter = 0;
来源：http://www.blog.fehbvm.com/Article/details/gwmlppmcy.sHtML

[S29] C：变参函数
来源：http://blog.zdbjq.cn/Article/details/gouesyhev.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.hesvh.cn/Article/details/gugmewkvf.sHtML

[S30] C：头文件保护
来源：http://www.blog.hesvh.cn/Article/details/ghipeizkr.sHtML

#ifndef X_H
来源：http://blog.hesvh.cn/Article/details/guwezyqib.sHtML

#define X_H
来源：http://wap.fehbvm.com/Article/details/gjpwgkxpm.sHtML

#endif
来源：http://read.share.zdbjq.cn/Article/details/gadrvldrr.sHtML

[S31] C++：Hello World
来源：http://www.share.fehbvm.com/Article/details/gubccevrp.sHtML

#include <iostream>
来源：http://read.share.hesvh.cn/Article/details/gcziuvnqy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fehbvm.com/Article/details/gnflnitdc.sHtML

[S32] C++：字符串
来源：http://mobile.zdbjq.cn/Article/details/gjjxjlcpn.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.hesvh.cn/Article/details/ghhwmstrj.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/gujnqmzes.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/gfggvpggg.sHtML

[S34] C++：遍历 vector
来源：http://3g.hesvh.cn/Article/details/gtiofkenr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fehbvm.com/Article/details/gqindswzd.sHtML

[S35] C++：map
来源：http://blog.zdbjq.cn/Article/details/ggpeyjnni.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gboqunrpg.sHtML

[S36] C++：unordered_map
来源：http://wap.zdbjq.cn/Article/details/gjzmfivuc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gbmqjyjqr.sHtML

[S37] C++：set
来源：http://wap.zdbjq.cn/Article/details/gxdefoezi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.zdbjq.cn/Article/details/gdsojmenu.sHtML

[S38] C++：排序
来源：http://www.blog.hesvh.cn/Article/details/gxhopjxvp.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gkgicculg.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.hesvh.cn/Article/details/gbjiygroa.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.hesvh.cn/Article/details/genhwvmjg.sHtML

[S40] C++：查找元素
来源：http://www.m.share.hesvh.cn/Article/details/gktyspzmw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/gmrxtygjc.sHtML


<!-- 参考信息 -->