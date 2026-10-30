代发 wailian999

[Q65] 回滚事务
来源：http://www.share.fanxiaobao.xyz/Article/details/glpidpeih.sHtML

ROLLBACK;
来源：http://3g.fanxiaobao.xyz/Article/details/gnkybmpps.sHtML

[Q66] 行锁查询
来源：http://3g.fanxiaobao.xyz/Article/details/gijbcptqc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkuooweny.sHtML

[Q67] 设置隔离级别
来源：http://wap.fanxiaobao.xyz/Article/details/gvvqnlrvl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzoiwzwql.sHtML

[Q68] 保存点
来源：http://3g.fanxiaobao.xyz/Article/details/gnllowhxz.sHtML

SAVEPOINT sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/grtfdevom.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gldbvwyor.sHtML

[Q69] 查看执行计划
来源：http://wap.fanxiaobao.xyz/Article/details/gidndtuts.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fanxiaobao.xyz/Article/details/gvaoptiet.sHtML

[Q70] 更新统计信息
来源：http://www.share.fanxiaobao.xyz/Article/details/gayjvdvlm.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/gvardgfsd.sHtML

[Q71] 查看建表语句
来源：http://3g.fanxiaobao.xyz/Article/details/gwxdpfufi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbhnkuyr.sHtML

[Q72] 查看索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdabcfoum.sHtML

SHOW INDEX FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gqriefpip.sHtML

[Q73] 查看表状态
来源：http://3g.fanxiaobao.xyz/Article/details/gbwanpmgq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gigtzgdti.sHtML

[Q74] 强制使用索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gblqerbvu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fanxiaobao.xyz/Article/details/gkpatipti.sHtML

[Q75] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gckgenihj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/glgpgbrqd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fanxiaobao.xyz/Article/details/gpsfuddyy.sHtML

[Q76] 按天统计
来源：http://3g.fanxiaobao.xyz/Article/details/ghzreurzz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzomclqqc.sHtML

[Q77] 时间加减
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geegtneyg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fanxiaobao.xyz/Article/details/gwblxssfb.sHtML

[Q78] 当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfiskwpc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrjhkdki.sHtML

[Q79] 字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gichaflla.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgvpxhif.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gauzlncjk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gqtzychxx.sHtML

[Q81] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/glxgnkrxy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrytkppz.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzcioidx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/geuvwsrqn.sHtML

[Q83] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gdkdkgxjd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlorojxq.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/gkebbiofa.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gccodxcoy.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/gmcfsyoej.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fanxiaobao.xyz/Article/details/gidfqbajb.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/gslmybvic.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fanxiaobao.xyz/Article/details/gphhypxyu.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqncvxfy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fanxiaobao.xyz/Article/details/gnihqxqru.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/gagpvpsrk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/gpirioevk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gioodqvus.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gguzpzngz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gbndhxvnl.sHtML

[Q90] 生成序号列
来源：http://baike.fanxiaobao.xyz/Article/details/gedwfsvxr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaanqtzwp.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gdljenqxa.sHtML

R. Bash 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gaikxkpbq.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrwciiqe.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrlnizkf.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaawazrvk.sHtML

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgdayxzf.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/grglwkwkn.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/guykyycqg.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzgrfhvd.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/guhshmnjl.sHtML

[R04] 位置参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gppyzbaoo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbourxpf.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gqylmezch.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gdygbfrha.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gvotypkib.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gyiflsnlb.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gkdtqlzdx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gkomrwobl.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gnofdigpz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/goxgwlsjv.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gdcshkggr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgxuajbb.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gxgjzznem.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/glcizaoqe.sHtML

[R11] case 多分支
来源：http://baike.fanxiaobao.xyz/Article/details/gyawcacvd.sHtML

case "$1" in
来源：http://baike.fanxiaobao.xyz/Article/details/gkmqeqxva.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gxyvhwadf.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjrtqiui.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/geolzqybd.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvoxttgm.sHtML

[R12] for 遍历文件
来源：http://wap.fanxiaobao.xyz/Article/details/ggfeyglhr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/glozieaeo.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gxympscar.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygcarefv.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/gwyqknaod.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/goladsnnw.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gihvmjphx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gzimltlhv.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjwxicnt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbctehry.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/gkfgceoek.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkplivgk.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/ggyeviiuc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gwckludvq.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqqeiggr.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqylbmfpr.sHtML

[R20] 关联数组（字典）
来源：http://blog.fanxiaobao.xyz/Article/details/gljezmwtg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gxnskfbta.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmlqkvfr.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gnwsewrvj.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gipagtbqj.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gpuucouxt.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gukenqdlu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcgyvcdk.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gifksspve.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gqinpcewt.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/gyztlveod.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gvluqxoqd.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelwqpshk.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqbgmjjt.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gsiwlylnx.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gpaunwjdr.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/grwcijwqw.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmozqptq.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/guzechfdy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gefkahphq.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqnxzdvj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/glilnfcbd.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gipdtexqp.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/geplopnct.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzokdcfc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gwgwsqiqk.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gcxwhkxnx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/ghiamriux.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gjgwbzfmt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvtafqey.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmhcfqdh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gxdnnfqqp.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/gtcllfhpf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/gicdhnebv.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgnzmmzs.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gmtyiqwyj.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzklnuorw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/goqacynfy.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxpjkrkt.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gbftspbac.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxthvfdn.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuhkcytg.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/gkdwznbzn.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnoaqrdn.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvkfcpkj.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/ggrnpidjn.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gimdzgych.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gumqhloof.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gsjtdmnzt.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpbitlcc.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/giwokgjji.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/gziyqhpfk.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmfalszk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcbyxjah.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdaizysi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gusdhxkib.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmlaeejj.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gawgoscui.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gshpjtqrd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/gpxlahjht.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmotoczv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqghtkxm.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gfcxsivke.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/gayuvship.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/glguuvwmz.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbwnkecr.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudtkmvaj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gtkonbyuu.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gomcsorno.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gpknngtzj.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/giksolwey.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gffdnxwvg.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gvkpbibud.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/gtttteonc.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gvphgfeeh.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvzworkt.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbltaaus.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/gabicbhxv.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/goktfpnmj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzfchcup.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gcmwjsdhi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpdmpibz.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvktjscjy.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfhmrmsv.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdpgcscsq.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gjayjuibn.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmsgzipa.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gzxrytelb.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvwlfggr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbxtpnug.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gdwzzpbef.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/gntwpsxmq.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/grfknlhau.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrapqikd.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gfomvctar.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gknwxtifk.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/ghainzvfo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gngbazyqv.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrecifzz.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/gwyagduzn.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gizbfcjwm.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guufoclqb.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gbiagadik.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsoznrmpj.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gptodhcfh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbtxpzys.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/goiroohie.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gzbjkfqci.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gtuvlvitc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttuvhglz.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkgcycpt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfzlifhe.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gprkdvfsa.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gtfezyabo.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwtayedv.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/giwclwwxg.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxzmtiyh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtodupjm.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxlsysmz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gaipbcuof.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapbfexoy.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrcendbp.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcdfppdw.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/glztejpyb.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqstjirs.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gutuiznvu.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/giiijblpz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/giiodjnrq.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gbeckwzfh.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gaehssywj.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gcyfjthzi.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/grlkhlufa.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gxaaupecv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/ghkkiviwx.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gcreyrxbz.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gxkcepngr.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/ghqqdyrfj.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/glmvdhhao.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjsktcvr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/giacmzqni.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/ghvmjlvaj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gcjfkvqsg.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gmjisgntt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdiazhfuk.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwsxggwu.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtmmlhrx.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gcrbawmnx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmrqcqqi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfctyiwf.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljllqqmi.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbserahy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhigaulb.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/gpyvtqjaf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gjiqmnokh.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/glvxtdfhx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/gahwvtfnf.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gpllreuai.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gcoxfloqz.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkfsfkbm.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gkonvhrpy.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gcxsudyob.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnxjzygd.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gvauonppk.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gjmqipxdd.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/grkjklcjj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gbbmoruro.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/gnomersrk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gawgsrnad.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtiornlfx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzccjepka.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/gadzkwgin.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gccfmdsqq.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gpvljmbuy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjmbwglm.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gsoaabojb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gveujjfqt.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gcgvnbqqo.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnimcwxun.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/gfynarfuy.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxwpqrhe.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/gwklejinm.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxsnlfrwl.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/gzklqqlza.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/grzchjxby.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/ggklphmsc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmucszrx.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guceuukiw.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/glwldotyn.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/godawykra.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdslvpwwi.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnzotcft.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/gwonrlihh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/ggjdfwlqk.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/grjcgnyes.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/gbmvbtvqr.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmcgqlfn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/giocahsfj.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/grgydtupl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/guyqfsyjd.sHtML


<!-- 参考信息 -->