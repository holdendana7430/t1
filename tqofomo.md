代发 wailian999

SHOW INDEX FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmjvjujm.sHtML

[Q73] 查看表状态
来源：http://read.share.fanxiaobao.xyz/Article/details/gekqfcife.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwarwilp.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmppsiuzo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhkfzwns.sHtML

[Q75] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbonqofhl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/guemkvrgw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/gwfyzziyv.sHtML

[Q76] 按天统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlncsqcw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fanxiaobao.xyz/Article/details/glgsvfpig.sHtML

[Q77] 时间加减
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfhpmxqv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhvmwpmm.sHtML

[Q78] 当前时间
来源：http://www.share.fanxiaobao.xyz/Article/details/goymeuywf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fanxiaobao.xyz/Article/details/githngujz.sHtML

[Q79] 字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/googqlnop.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtafmxfa.sHtML

[Q80] 字符串截取
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfmmabuj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gnzwzocro.sHtML

[Q81] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gymmabfam.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gksohlkrf.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgalyiad.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gauopzlpu.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/genyeqsdz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtyuzdbex.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fanxiaobao.xyz/Article/details/gknsvtalz.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/glkufwull.sHtML

[Q85] 数值取整
来源：http://baike.fanxiaobao.xyz/Article/details/gjxzjwyrh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fanxiaobao.xyz/Article/details/gyfnnpiqf.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fanxiaobao.xyz/Article/details/gugkvyfqd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqhxoqyw.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwehffqu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxzvhtdw.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fanxiaobao.xyz/Article/details/gvonsrggy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvulkcfa.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzeumpir.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gxygekztq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gdpyapmil.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhbneply.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gffzcihjw.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gvknazhwd.sHtML

R. Bash 专题
来源：http://blog.fanxiaobao.xyz/Article/details/galghygdl.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gpxoufvac.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gtnqpadol.sHtML

#!/usr/bin/env bash
来源：http://m.share.fanxiaobao.xyz/Article/details/glkmtwhkg.sHtML

set -euo pipefail
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwghlwav.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/gzlpjhald.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gsogrjurq.sHtML

[R03] 只读变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gevqxowbi.sHtML

readonly PI=3.14
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmmnaioj.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdnqjbbv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtfyarer.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazlsllej.sHtML

name="${1:-default}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpudegden.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcuocqpgk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/grbmdrmmo.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpovvlsqe.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gliejhjqa.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgkdtpkn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gxibehewg.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/ghbgevmiq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwjcxrsf.sHtML

[R10] 正则匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkjcmjfs.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gweatblts.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/gomtnymcy.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gijawdcdg.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gopugnins.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgwfhlxi.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpemptptk.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/gewszzdrd.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwidyazv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxhcdfxa.sHtML

[R13] for 计数循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gupiiznmk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gjijcyhdm.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwbbjvdv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gjqfudphv.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/greibnrxz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gnyerusmc.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gdzrurhev.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gddwiooji.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/gkayxrbvj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczdvqpig.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjnlqihw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gsypiitlh.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrwbgunr.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsemfefib.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/girxxaevi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gcnnhesei.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gykhfjbvh.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gszvfuddo.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gicjpwicz.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gyhlrqlrz.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gilpgmvcl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gwmlvtvzu.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/glkiterfb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/gblxqpwwu.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/gdmubtjpv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmurhlth.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfldvfwf.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/gifkerxsd.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/gxlolhbmf.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gihnhyadw.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpvbtonm.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujlshkvk.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtufqnwo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gtswpnufh.sHtML

[R30] 函数返回状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gbalcjvql.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxyzlrni.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gzftrxfir.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmuwksfya.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvsoegtt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/genuwpbtl.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gklbiwfup.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/ghltzdgje.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gmddcuafz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzybyalsv.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrjxmuvn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpuwunreh.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvewirev.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpedlojd.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrfyddec.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/glawszkjp.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gvggixynm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gkrvmapnr.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjkjhilv.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtfjiunr.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gucjumili.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grghgbkdm.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gjeeamgiq.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/ggictgcsb.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpspztfah.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gwpppqzvj.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdnsawme.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gbpoushyg.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/ggbocvlbc.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gckegdjgr.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpaprqrq.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/grdnutjmk.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyzgwzuf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlpmqmix.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/gysjdeoby.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjroydck.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganyduwub.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/grnuasjcw.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gfhsstecz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/ghgjnjzeo.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/grugqntti.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gtygaewmb.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkeuqame.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvwdbyij.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxvtdshn.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gwyrqsohj.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfdjlbfy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslyssxol.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsogiwza.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gdrmnfjro.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghocntlhl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjgdbbqx.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfdvsqkn.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gfotgahdn.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/gbncaqtlb.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gttvsurkg.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/ggojbxdcl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxqnqbal.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gxniicxcp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gedkeqiuw.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/griwkduoo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gbiytriqd.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/guvrjfyhj.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gdngwesrm.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gjgyowvxm.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjufkdghp.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbqqueid.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gdrqjeodj.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwiteqkb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gysrttmzg.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gzbksogiw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghuprvnlw.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdidrcpmp.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjipusneq.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/glizknync.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpnjmxee.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gbffjtdrs.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/giajtllzu.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gnbszcehk.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gweydwncw.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukumbwon.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gtremfbxl.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdoxgbujb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqodhqha.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/guffggiaw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvorqyae.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfnxsxdn.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyvkkvzk.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqobjipa.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gndiravyf.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwuxmfvl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbkmcxbr.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezjcfxjj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmdcrvet.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjzoqoaw.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfdghmcl.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/glwzwmyuj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqidjzyb.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gqeolqasm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gxsupihkv.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gsvlgzrhw.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/glkvtasjg.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/goiwudllm.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gjssaexgr.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcseopmx.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gxdchoymd.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnjrtuhp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gddappzxy.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/grkwzasjj.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhqhekqf.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnqemrvi.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggumdrfgj.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gygnhnepo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsaaphfco.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjttygkio.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gghohhxwt.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcwncoed.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gksycoqjk.sHtML

[S07] C：数组遍历求和
来源：http://blog.fanxiaobao.xyz/Article/details/gefpkrkwg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/guqthuszy.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxamaegz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmocdrlvy.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhxgotsz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gigmenwll.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gxngwslhw.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/glgofdtuc.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvbaafui.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gercfpire.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gnlletgwx.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gbanhgvth.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gibpzlxrz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtcabrxtq.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmzbqtzn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/glzgyogqe.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gizetqxor.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyvcjacr.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gfxafswnp.sHtML

(double) a / b
来源：http://blog.fanxiaobao.xyz/Article/details/glfcaylvs.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/glkjmvkut.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtiuhipom.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gtiwiuhlh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzrmpbxb.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrmgsdpz.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/grshzlxvb.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gujgfauge.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdznhdhcw.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/gedvuakyy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gtgobuddv.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gghaekqup.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmryrqwww.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdwbifex.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamwlwlzq.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzivbtzc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghphjfwxm.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gxakkicdr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/gcxpxutfz.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gkwrcwavo.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbvhgrdd.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/gfwmrqvqo.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/geqksbkxg.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/glbwakfvz.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/ganylirac.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcgtwcez.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gyhcesywp.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gleuigqgg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfejuukoq.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/grhfjbzxb.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gglmafwlx.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gizlozfvt.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guseaimea.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghsvptjx.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gwdgpuknb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gupqoucaa.sHtML

[S32] C++：字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gyouhtbxb.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwlqarca.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmysodwy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzurvwuyu.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkvkyuzl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/geunbwrpr.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/gmsjqwqan.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/glqbxxoip.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxolgwold.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/geablmcyy.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gdhhdquar.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgyrkdmq.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccocxdmg.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifrsaeiu.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkuadono.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdwfsasq.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gkuysrzaa.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsuydvpxi.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gojonnqzq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqoqvron.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gggvdqhut.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztyecbcc.sHtML


<!-- 参考信息 -->