代发 wailian999

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/genmkrimz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/glkjkkhbe.sHtML

[Q77] 时间加减
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhzjvvxf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fanxiaobao.xyz/Article/details/gqvbuoodw.sHtML

[Q78] 当前时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gdohwufdg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fanxiaobao.xyz/Article/details/grqjqaisx.sHtML

[Q79] 字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gfoxiicau.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fanxiaobao.xyz/Article/details/gbaqwlsyl.sHtML

[Q80] 字符串截取
来源：http://read.share.fanxiaobao.xyz/Article/details/gqyonolpz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gblknfkmo.sHtML

[Q81] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/ggheplkvo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtiquvjke.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpqutxnk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozsgphru.sHtML

[Q83] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjanirik.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/ggxvxsgat.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/gyhbdtbtr.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gbijtyqtm.sHtML

[Q85] 数值取整
来源：http://3g.fanxiaobao.xyz/Article/details/ggedrzlnx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fanxiaobao.xyz/Article/details/gfeetjnqv.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fanxiaobao.xyz/Article/details/gcoqouygl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/gztsinoiw.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdnjcwua.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fanxiaobao.xyz/Article/details/gjjrwvdpd.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geypqgzhb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcgrankb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gixindyoe.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gdujnmcdu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqyagkck.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/gkvgkgjcb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/gkjdyfdsm.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegswfpew.sHtML

R. Bash 专题
来源：http://wap.fanxiaobao.xyz/Article/details/grqjyavgm.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gqitesrpu.sHtML

[R01] shebang 与严格模式
来源：http://blog.fanxiaobao.xyz/Article/details/glzbmslda.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/gwtazttxz.sHtML

set -euo pipefail
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwumcgju.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwwxbnah.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/gnukxmdfr.sHtML

[R03] 只读变量
来源：http://mobile.fanxiaobao.xyz/Article/details/ghptwkfvv.sHtML

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/gnnajkmqq.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/gyhalsvzo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fanxiaobao.xyz/Article/details/gbcgcinjd.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gnvsevbhf.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/gfcigeeil.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/ggylfcubh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkhlidlu.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gciuoitgf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/glpbvfomt.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/grtwolrmm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/grxwtnfaj.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/glawbxtem.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfynfejza.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gycfhffwa.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gopolxpvo.sHtML

[R11] case 多分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsgovhvi.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gevtaqnrn.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/golrbjmsf.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/grceewgpp.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gembamsfi.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvstodrm.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/gsxcgmcsq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/ghiiabvij.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/gyjzazilu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkhfigvy.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbaztmpbs.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxcmwauc.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gvbvmjpik.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gswxprhwc.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/glucnygup.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gmdbjanrm.sHtML

[R17] 数组定义与取值
来源：http://baike.fanxiaobao.xyz/Article/details/gqndrwvok.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gflnnnqcg.sHtML

[R18] 遍历数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gdcilrryg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnpyhmzg.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/giolzdlrj.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gewlccfvy.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/gukwghbzr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/ggckqzrsn.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gsmcsfrru.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/grsdmdvpi.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/glyqcgmlq.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzabeomhg.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkubtaed.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqqrmjiw.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwhkqmrs.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gllwhjpyq.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/gvbdoimpg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdftjmlmt.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gedkedkmo.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkchszkhj.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdgdqbft.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdddvovym.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghddynhqt.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/gmtuiqbjt.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbojftxq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/gcultlgyo.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gnfemlyei.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/graylqzha.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/giamyjilm.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsotetsnc.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/ghtywjyvf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxtjhsbll.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpplcurn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gsocvfaft.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/gdojynpfm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gazpsnzdm.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gzmdcuavj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gvwfjxveg.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/gprynubmz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/gkjuvcpfp.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfeququsu.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gudqwekfz.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgnjoysx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gxamjcbdt.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/gleehmlbo.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gqadccbwh.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/gboxvwydp.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdutzoyf.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbkvmxoh.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gouzmesgg.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhldscsr.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gbtdzscme.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/geikwfqwu.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gujyephuw.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/grsiejwhn.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrfeblgo.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/grparkabv.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gnywhfqgo.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkawettn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gqxkrfnyf.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gifcpuyuk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpusofqe.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gzmdhwout.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwukxrjf.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gjakoqubt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqrlwsis.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/ghfktzmwc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmjicwum.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/goxdjtvxv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/geyanrbsu.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gsmcqgzti.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gexwzbnkk.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzrwkpha.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/gscruqzdc.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gjagljpdu.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/glcfkicbr.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmionnube.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/glfavxgud.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gbjixzljn.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/grugwfbqf.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/gyydldfsx.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gulpnsjwk.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gstpzzivc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/ghtwrqmxl.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxnmkysw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gossjzduv.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwvsidhs.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/ghzvgibqp.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgdbtvpp.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/ghgunnhrb.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gfavwivgk.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gmobefalv.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guadfhfna.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gusczcnka.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/ginauumcd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/gjxjjqems.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gnapmlbbl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/gmicpekey.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwuuylhwi.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtncktmpz.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gwjuisnyw.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/gbyclizgr.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gromkddmb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gjajavhxb.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/goqbyxaby.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gnhcspbem.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/ghsugqbcl.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gjzcfwshv.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzgjlarw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxccgyri.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqofyzna.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gfyyzqocn.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqfschqk.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gpicabjsk.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gvclrdcec.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjegfuji.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gevguzmll.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmerhrgxx.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gqiuydstb.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gevjamemv.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gmepyjpya.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbpyfeuy.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gievcytxi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gdsewnwcw.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gxmoardry.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgzdgigt.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gadtrcizo.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqgeiuba.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gurdflrwi.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gwbhorpjz.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gdmabfwmm.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gztfzxvzk.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gerdvxzng.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqegdompy.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gbroepnlu.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gledibuou.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsihhrxqi.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/gifdfdxpd.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/ghcyrbfxb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gbciecdbd.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gbbqpkull.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/govyxotyo.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnonzqvb.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gwcovthqo.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/grqjxyqmy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/grknvtnmc.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gllxmjrzx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gswtvjghe.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/glaqtjfrq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfxrzjsk.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gozxdlond.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gelephmnp.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gzcrvwoso.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/gkzkypncq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbsenpjgz.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gmjpjsgvk.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gbfahbmez.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxluhirz.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/gxpysotrt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/guwtwmlxa.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrrgpnap.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjuicsfdd.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrssfitu.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gqnavrwli.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/ggjqdegah.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/ggiytcvod.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdaswzuu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/grstseeeb.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehkdsjso.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimueykkn.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gcruxzmkr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gzczcnswi.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gaeoiuixc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gobpxtgbt.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/ghtwbvbpv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhskwlph.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywnbtthk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/glihbzxip.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/gztomwnla.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gyltcksjv.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/grhicjvzi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gmgrnjrdj.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwvwpdeg.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfgnnxlh.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/grlzjsacr.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gaetqaiei.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/ghbjxxzqg.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gupadfwgu.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gkisntzwx.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyondklq.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmtrpyco.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwfkqxqn.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gdiaxgnec.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxqckkqt.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gtgpiqmsj.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/gegeiakps.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gupgwgngy.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gvfxcrrhp.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gannidwed.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrvhvycp.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxjgslmq.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/gxixxqxsb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gnhxdgljr.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/gmqpqfetp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/girunontg.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/glusedfpj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gckyapgjj.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/ghjsidlqi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspnjowxq.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gbwwyqttt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gvtfonzvi.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gnjmnbqwe.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdolcjtx.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gepcbejxx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/gyzhexuqd.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gplbajqhj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppwumxza.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/ggodqovhh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/goujbzfsx.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwlnrack.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshgsgrgb.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gjbroqrce.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/gakllhgna.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnsdrkstf.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/guithdshp.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/gmhquaipg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmfyjunz.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdahlkfto.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmksmklz.sHtML


<!-- 参考信息 -->