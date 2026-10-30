代发 wailian999

ROLLBACK TO sp1;
来源：http://3g.zdbjq.cn/Article/details/gnbtefhog.sHtML

[Q69] 查看执行计划
来源：http://blog.zdbjq.cn/Article/details/griothbzm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.zdbjq.cn/Article/details/gmkvwtjgz.sHtML

[Q70] 更新统计信息
来源：http://m.share.zdbjq.cn/Article/details/gxkeadiex.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fehbvm.com/Article/details/ghwzhpzvd.sHtML

[Q71] 查看建表语句
来源：http://baike.zdbjq.cn/Article/details/gvptyypyz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fehbvm.com/Article/details/grlookvsi.sHtML

[Q72] 查看索引
来源：http://mobile.zdbjq.cn/Article/details/gvycidnni.sHtML

SHOW INDEX FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gjfbqheyd.sHtML

[Q73] 查看表状态
来源：http://www.blog.hesvh.cn/Article/details/gkflwkpki.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.hesvh.cn/Article/details/gpuatqibw.sHtML

[Q74] 强制使用索引
来源：http://read.share.hesvh.cn/Article/details/gqikgvqwv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fehbvm.com/Article/details/gjviimhnv.sHtML

[Q75] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gqhurlcqq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.zdbjq.cn/Article/details/grapzbwpd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fehbvm.com/Article/details/gcrmagyjw.sHtML

[Q76] 按天统计
来源：http://3g.hesvh.cn/Article/details/ggsjscwyn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fehbvm.com/Article/details/ggciezwnw.sHtML

[Q77] 时间加减
来源：http://m.share.hesvh.cn/Article/details/goryzpuzz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.zdbjq.cn/Article/details/gtezneyzg.sHtML

[Q78] 当前时间
来源：http://wap.hesvh.cn/Article/details/glzomonso.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fehbvm.com/Article/details/gtrcbvvff.sHtML

[Q79] 字符串拼接
来源：http://blog.zdbjq.cn/Article/details/gxhjusbrx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.zdbjq.cn/Article/details/gjjtgxiow.sHtML

[Q80] 字符串截取
来源：http://read.share.hesvh.cn/Article/details/gddtzhfmb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gnlpwmbft.sHtML

[Q81] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gpvxdsejy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.hesvh.cn/Article/details/ghiucrckz.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fehbvm.com/Article/details/gverrqiuw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gzvufmadl.sHtML

[Q83] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gtpizddna.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/glpzivmur.sHtML

[Q84] 去除首尾空格
来源：http://baike.zdbjq.cn/Article/details/gepivezvs.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gdjhwhukc.sHtML

[Q85] 数值取整
来源：http://read.share.fehbvm.com/Article/details/gnybuvbqz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.hesvh.cn/Article/details/gujntnexo.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.hesvh.cn/Article/details/gsagsjbvk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.zdbjq.cn/Article/details/gziwafpbz.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.zdbjq.cn/Article/details/gpulxpccu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/glziousqt.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fehbvm.com/Article/details/gzjbgasbh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.zdbjq.cn/Article/details/gglpllcho.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gwckolbrb.sHtML

[Q89] 判断表是否存在
来源：http://baike.hesvh.cn/Article/details/ghirgonky.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.zdbjq.cn/Article/details/gqdznhrze.sHtML

[Q90] 生成序号列
来源：http://baike.zdbjq.cn/Article/details/ggbadqvel.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fehbvm.com/Article/details/gjvdiltgg.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gewgvzrpm.sHtML

R. Bash 专题
来源：http://wap.zdbjq.cn/Article/details/gzaslsyct.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gglyljwkq.sHtML

[R01] shebang 与严格模式
来源：http://blog.fehbvm.com/Article/details/gssntzxoa.sHtML

#!/usr/bin/env bash
来源：http://blog.hesvh.cn/Article/details/gcrruergi.sHtML

set -euo pipefail
来源：http://read.share.zdbjq.cn/Article/details/gpjzxldha.sHtML

[R02] 变量赋值与使用
来源：http://mobile.zdbjq.cn/Article/details/gpvidqecx.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/gfsnodiic.sHtML

[R03] 只读变量
来源：http://m.share.fehbvm.com/Article/details/ghsompipk.sHtML

readonly PI=3.14
来源：http://www.m.share.zdbjq.cn/Article/details/gvxqcahhv.sHtML

[R04] 位置参数
来源：http://blog.hesvh.cn/Article/details/gngeqixwo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/gjucgrdpl.sHtML

[R05] 参数默认值
来源：http://wap.zdbjq.cn/Article/details/glwmtwdgb.sHtML

name="${1:-default}"
来源：http://read.share.zdbjq.cn/Article/details/gfndpxfhd.sHtML

[R06] 判断命令是否存在
来源：http://m.share.zdbjq.cn/Article/details/gsynyffup.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/grvfuwrpn.sHtML

[R07] if 判断文件
来源：http://wap.zdbjq.cn/Article/details/grkutxxxk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fehbvm.com/Article/details/gdkzgqbsf.sHtML

[R08] 数值比较
来源：http://mobile.zdbjq.cn/Article/details/gmihwxkny.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.zdbjq.cn/Article/details/gwhhcckee.sHtML

[R09] 字符串比较
来源：http://baike.fehbvm.com/Article/details/ginyvqbdq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.zdbjq.cn/Article/details/ghfodvmni.sHtML

[R10] 正则匹配
来源：http://m.share.fehbvm.com/Article/details/gwoqikrqm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/ghovefatr.sHtML

[R11] case 多分支
来源：http://read.share.fehbvm.com/Article/details/gqqcnhjmc.sHtML

case "$1" in
来源：http://baike.hesvh.cn/Article/details/gummusnqa.sHtML

start) echo "启动" ;;
来源：http://wap.fehbvm.com/Article/details/gcbtbolrh.sHtML

stop)  echo "停止" ;;
来源：http://read.share.hesvh.cn/Article/details/gsjtqfajh.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/ghkoutdmk.sHtML

esac
来源：http://baike.hesvh.cn/Article/details/gyhwkscwb.sHtML

[R12] for 遍历文件
来源：http://mobile.fehbvm.com/Article/details/gzdayywui.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.hesvh.cn/Article/details/gbbvylaew.sHtML

[R13] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/ghxoomrxu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gfxzhbqtr.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/gvfpaspdj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gwwrhxoew.sHtML

[R15] while 逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gmmuqdlch.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.hesvh.cn/Article/details/gximiozqy.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/gblfryzvk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/glstehyzh.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/ghcfzuzfl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.zdbjq.cn/Article/details/gnwbvhxqk.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gbutcwksn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/gxlxpcjdx.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gcaakophv.sHtML

echo "${#arr[@]}"
来源：http://wap.zdbjq.cn/Article/details/gppsvyfut.sHtML

[R20] 关联数组（字典）
来源：http://www.share.zdbjq.cn/Article/details/grvvobogw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.zdbjq.cn/Article/details/gehhiaycv.sHtML

[R21] 字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gxgmzwpsr.sHtML

echo "${#s}"
来源：http://3g.fehbvm.com/Article/details/getunlmlm.sHtML

[R22] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gereohzyz.sHtML

echo "${s:0:5}"
来源：http://www.share.zdbjq.cn/Article/details/gdvyiwsmv.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/goazsnxpr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/gonwrtsgl.sHtML

[R24] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gqrmbxyup.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.hesvh.cn/Article/details/galudmbzb.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fehbvm.com/Article/details/gxjaibgue.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.hesvh.cn/Article/details/gxhmpucyx.sHtML

[R26] 命令替换
来源：http://baike.hesvh.cn/Article/details/ghpujkhfg.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.zdbjq.cn/Article/details/gonrjjldl.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/gwcxfkpws.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.zdbjq.cn/Article/details/gkncgpnxd.sHtML

[R28] 浮点运算
来源：http://www.m.share.hesvh.cn/Article/details/gmjezwoty.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.zdbjq.cn/Article/details/gzxztaxfm.sHtML

[R29] 定义函数
来源：http://wap.hesvh.cn/Article/details/gwthdjvkk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fehbvm.com/Article/details/gfecadyzu.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/gsqwrpmxm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fehbvm.com/Article/details/gtxtupozb.sHtML

[R31] 局部变量
来源：http://baike.zdbjq.cn/Article/details/gcakyywrg.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/gqreueisl.sHtML

[R32] 参数个数校验
来源：http://3g.hesvh.cn/Article/details/gukunwria.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gdjxjztmp.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fehbvm.com/Article/details/gzfahbmdr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.hesvh.cn/Article/details/gudkmficu.sHtML

[R34] 退出时清理
来源：http://www.share.fehbvm.com/Article/details/gdmsjgchs.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gcwsdbtdw.sHtML

[R35] 后台执行并等待
来源：http://www.share.zdbjq.cn/Article/details/gqptgqxul.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fehbvm.com/Article/details/gcltabqpj.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/gpmntbwfd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.zdbjq.cn/Article/details/glfdfkhkw.sHtML

[R37] 把输出赋给变量
来源：http://baike.fehbvm.com/Article/details/goqazhrir.sHtML

files=$(ls -1)
来源：http://read.share.hesvh.cn/Article/details/ghekpmqlv.sHtML

[R38] 管道串联
来源：http://www.share.zdbjq.cn/Article/details/gbnqozhft.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.hesvh.cn/Article/details/gghaiqewb.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fehbvm.com/Article/details/gxtgoxqgo.sHtML

cmd > out.log 2>&1
来源：http://www.share.zdbjq.cn/Article/details/ggjekhzcd.sHtML

[R40] 追加写日志
来源：http://3g.hesvh.cn/Article/details/gjhlfutob.sHtML

echo "log" >> out.log
来源：http://wap.zdbjq.cn/Article/details/gpwrvuaau.sHtML

[R41] 丢弃输出
来源：http://www.blog.hesvh.cn/Article/details/gplfdygcr.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gvywdstqn.sHtML

[R42] 输入重定向
来源：http://3g.hesvh.cn/Article/details/ggdwzpawm.sHtML

wc -l < a.txt
来源：http://www.share.zdbjq.cn/Article/details/gllcrqath.sHtML

[R43] 按名字查找文件
来源：http://blog.hesvh.cn/Article/details/gtrzywboq.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/ggbuocrov.sHtML

[R44] 按修改时间查找
来源：http://www.share.fehbvm.com/Article/details/gbwklibyg.sHtML

find . -mtime -7 -type f
来源：http://www.share.fehbvm.com/Article/details/gojkuhupb.sHtML

[R45] 批量删除
来源：http://baike.zdbjq.cn/Article/details/gbzsjylib.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fehbvm.com/Article/details/geiqaulxv.sHtML

[R46] 递归替换文件内容
来源：http://blog.fehbvm.com/Article/details/gvnqzrqoh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.zdbjq.cn/Article/details/gqfaedclo.sHtML

[R47] sed 单行替换
来源：http://wap.hesvh.cn/Article/details/gyadfivck.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gntfdgugf.sHtML

[R48] awk 取指定列
来源：http://m.share.fehbvm.com/Article/details/gktisxpkc.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gjplpsrhe.sHtML

[R49] awk 带条件
来源：http://m.share.fehbvm.com/Article/details/gyqyzwdfa.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.zdbjq.cn/Article/details/gwhquwpas.sHtML

[R50] awk 求和
来源：http://blog.zdbjq.cn/Article/details/gostfrbtk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gjqjzujms.sHtML

[R51] 排序去重取前几
来源：http://blog.fehbvm.com/Article/details/gvyxnpbbx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/gcqjgppxa.sHtML

[R52] 统计行数
来源：http://read.share.hesvh.cn/Article/details/gyaiqwrvd.sHtML

wc -l a.txt
来源：http://read.share.hesvh.cn/Article/details/gvpeiecah.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fehbvm.com/Article/details/gtzbyltta.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.zdbjq.cn/Article/details/gapvtxmxp.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/gocszdbun.sHtML

diff a.txt b.txt
来源：http://www.share.zdbjq.cn/Article/details/gusidzgrv.sHtML

[R55] 压缩与解压
来源：http://mobile.hesvh.cn/Article/details/gylafemfo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/gihcyguvu.sHtML

[R56] 远程拷贝
来源：http://blog.zdbjq.cn/Article/details/gzwwvipdb.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/giyzbcsql.sHtML

[R57] 远程执行命令
来源：http://blog.hesvh.cn/Article/details/gdfcleazr.sHtML

ssh user@host 'uptime'
来源：http://baike.fehbvm.com/Article/details/gqtgepmmf.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/gaphpgbuz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/gqietjwmn.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/glvceevix.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.hesvh.cn/Article/details/gvlzvyycu.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gfraboesi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fehbvm.com/Article/details/gogvihmqb.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/gppqxrynn.sHtML

df -h;  du -sh *
来源：http://3g.zdbjq.cn/Article/details/gelpdhsil.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fehbvm.com/Article/details/gnorrvigm.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gzlcpudwq.sHtML

[R63] 内存与进程
来源：http://blog.hesvh.cn/Article/details/gokltxfdy.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fehbvm.com/Article/details/gnabgljvg.sHtML

[R64] 结束进程
来源：http://blog.zdbjq.cn/Article/details/ggfihxlaj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fehbvm.com/Article/details/gvxepfdcn.sHtML

[R65] 查看端口占用
来源：http://read.share.hesvh.cn/Article/details/glhlddhmw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.zdbjq.cn/Article/details/ggshfkowq.sHtML

[R66] 定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gmncsasvr.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fehbvm.com/Article/details/gnqgqbjdu.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.zdbjq.cn/Article/details/gidyaqpao.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/gedgfhzpl.sHtML

[R68] 计算文件校验值
来源：http://mobile.fehbvm.com/Article/details/gzevfwgqa.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fehbvm.com/Article/details/ggmkimyob.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/gcfkzstbd.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/ghkfktono.sHtML

[R70] 时间戳与互转
来源：http://wap.zdbjq.cn/Article/details/gkdujqjaq.sHtML

date +%s;  date -d @1700000000
来源：http://wap.hesvh.cn/Article/details/gaqrweyoo.sHtML

[R71] 日期格式化
来源：http://baike.hesvh.cn/Article/details/galcqscqo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/glvpwmksv.sHtML

[R72] 等待端口就绪
来源：http://mobile.fehbvm.com/Article/details/gtymzpadr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gpsmfrhbu.sHtML

[R73] 分割大日志
来源：http://www.share.fehbvm.com/Article/details/gixvwaeaw.sHtML

split -l 1000 big.log part_
来源：http://m.share.zdbjq.cn/Article/details/guyxqldla.sHtML

[R74] 批量重命名
来源：http://blog.hesvh.cn/Article/details/goiywbkaw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.zdbjq.cn/Article/details/gtiginuyf.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/gfpeggoyn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.zdbjq.cn/Article/details/gtynytitu.sHtML

[R76] 使用临时文件
来源：http://baike.zdbjq.cn/Article/details/gmxpxpbtl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/geqycfekh.sHtML

[R77] 读取用户输入
来源：http://read.share.fehbvm.com/Article/details/gfxdkhnhm.sHtML

read -rp "请输入: " ans
来源：http://3g.hesvh.cn/Article/details/gdurvrpul.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/gfqarmftl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.zdbjq.cn/Article/details/gdcecilfu.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/ggerbqfeu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.zdbjq.cn/Article/details/gzvlvfrym.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fehbvm.com/Article/details/gvuzkdpsh.sHtML

time ./run.sh
来源：http://read.share.fehbvm.com/Article/details/gskfgcipx.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzajvingk.sHtML

S. C / C++ 专题
来源：http://www.m.share.fehbvm.com/Article/details/ghpsvuooo.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmsaxnjwp.sHtML

[S01] C：Hello World
来源：http://baike.fehbvm.com/Article/details/gnehcdjax.sHtML

#include <stdio.h>
来源：http://read.share.hesvh.cn/Article/details/gxyncjosx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.hesvh.cn/Article/details/glwwsruxh.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/gecvtmvft.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/gzdxbnbji.sHtML

[S03] C：读入整数
来源：http://www.m.share.hesvh.cn/Article/details/grawsqjnv.sHtML

int x; scanf("%d", &x);
来源：http://www.share.zdbjq.cn/Article/details/giombyffx.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/grahnwxcs.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/grdmisdxv.sHtML

[S05] C：字符串长度
来源：http://blog.hesvh.cn/Article/details/glxgjgnzm.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/gpxewdwac.sHtML

[S06] C：字符串比较
来源：http://m.share.hesvh.cn/Article/details/gyfzokrvl.sHtML

strcmp(a, b) == 0
来源：http://www.share.fehbvm.com/Article/details/gzlxuozwr.sHtML

[S07] C：数组遍历求和
来源：http://m.share.hesvh.cn/Article/details/gipkgvdtf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fehbvm.com/Article/details/ggxxtsyku.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.zdbjq.cn/Article/details/geibtiyua.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/gcmrarhrr.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.hesvh.cn/Article/details/gmgsbcsze.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/gqqlvtnsw.sHtML

[S10] C：指针与解引用
来源：http://blog.zdbjq.cn/Article/details/giqakolqq.sHtML

int *p = &a;  *p = 5;
来源：http://blog.hesvh.cn/Article/details/gzlifikdk.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/ggeerrcpl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/gdgeqiavu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.zdbjq.cn/Article/details/gemzssrnm.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/gytcwpbum.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/gplcuxwnv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gcpbfburl.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/gicqalcjc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fehbvm.com/Article/details/gxgdlnmds.sHtML

[S14] C：枚举
来源：http://www.share.zdbjq.cn/Article/details/gcquitzqz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/guimyejtv.sHtML

[S15] C：类型转换
来源：http://www.share.fehbvm.com/Article/details/gnnhayllr.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/golsqidgd.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/giozkegtk.sHtML

x |= (1 << 3);
来源：http://www.share.fehbvm.com/Article/details/glfykylui.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gbpaoujaq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/gxmbpkgqm.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/giqurmvgw.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/gebnbxtnb.sHtML

[S19] C：快速排序
来源：http://m.share.fehbvm.com/Article/details/gnlbmfchy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/guavyrwmg.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/gkqgsfqpy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gicavlxov.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gdtyzxvxb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fehbvm.com/Article/details/gtibpldxy.sHtML

[S22] C：字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/gcukehrpf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.zdbjq.cn/Article/details/gqnzbjelg.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/gbczmgtjt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.hesvh.cn/Article/details/ghdrojrkd.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/goljmzkvh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/geuqipjql.sHtML

[S25] C：内存拷贝
来源：http://3g.fehbvm.com/Article/details/gvilkzynm.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fehbvm.com/Article/details/gravmdmln.sHtML

[S26] C：内存清零
来源：http://read.share.hesvh.cn/Article/details/gwpbylynd.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.zdbjq.cn/Article/details/glizwtzem.sHtML

[S27] C：定义常量
来源：http://m.share.zdbjq.cn/Article/details/glciglijz.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gsfrusrai.sHtML

[S28] C：静态变量
来源：http://3g.fehbvm.com/Article/details/gleueeonv.sHtML

static int counter = 0;
来源：http://www.blog.fehbvm.com/Article/details/gviqfbclv.sHtML

[S29] C：变参函数
来源：http://www.m.share.fehbvm.com/Article/details/gatvxmvfh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/geindqywy.sHtML

[S30] C：头文件保护
来源：http://read.share.hesvh.cn/Article/details/gywchtyli.sHtML

#ifndef X_H
来源：http://3g.zdbjq.cn/Article/details/gzchtqicz.sHtML

#define X_H
来源：http://www.share.fehbvm.com/Article/details/grrmghxmu.sHtML

#endif
来源：http://blog.hesvh.cn/Article/details/gowraxfnd.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/gdwjbadao.sHtML

#include <iostream>
来源：http://www.blog.zdbjq.cn/Article/details/gaimvltip.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.hesvh.cn/Article/details/girzcwqys.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/ghbsoftds.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.hesvh.cn/Article/details/gcxvkkrzy.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/gkokqnkzd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.hesvh.cn/Article/details/gqnvsvtxn.sHtML

[S34] C++：遍历 vector
来源：http://read.share.hesvh.cn/Article/details/gvncmsjmh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.hesvh.cn/Article/details/ggyfyhuyb.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/gtydvtghe.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gbgpbjdww.sHtML

[S36] C++：unordered_map
来源：http://www.share.hesvh.cn/Article/details/gnvqlgxak.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/goalbmlij.sHtML

[S37] C++：set
来源：http://blog.hesvh.cn/Article/details/gszhzxxvz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/gmnhndlwx.sHtML

[S38] C++：排序
来源：http://www.share.fehbvm.com/Article/details/gqkflqiek.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.zdbjq.cn/Article/details/gfyorjqzy.sHtML


<!-- 参考信息 -->