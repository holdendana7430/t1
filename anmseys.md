代发 wailian999

[Q61] 移动平均
来源：http://m.share.zdbjq.cn/Article/details/gebtomohd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gmsjxzewc.sHtML

[Q62] 分组占比
来源：http://www.blog.zdbjq.cn/Article/details/glszjykpn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gimzbfasm.sHtML

[Q63] 开启事务
来源：http://www.m.share.hesvh.cn/Article/details/grlbqxwos.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fehbvm.com/Article/details/gvbdmpgmj.sHtML

[Q64] 提交事务
来源：http://blog.fehbvm.com/Article/details/gqnrrrtor.sHtML

COMMIT;
来源：http://www.m.share.zdbjq.cn/Article/details/gwtmtoixf.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/gxmyqpyez.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/gkmproftx.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/gmzjxmoba.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fehbvm.com/Article/details/gqoseogul.sHtML

[Q67] 设置隔离级别
来源：http://www.share.zdbjq.cn/Article/details/ghpjsassu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.zdbjq.cn/Article/details/gjeuqwsni.sHtML

[Q68] 保存点
来源：http://3g.zdbjq.cn/Article/details/gpsgoqphq.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/gxboyuxyn.sHtML

ROLLBACK TO sp1;
来源：http://m.share.hesvh.cn/Article/details/gdxkvqenq.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/geiumdhsq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.zdbjq.cn/Article/details/gzrlsnlbo.sHtML

[Q70] 更新统计信息
来源：http://mobile.fehbvm.com/Article/details/gangaixmj.sHtML

ANALYZE TABLE users;
来源：http://www.blog.hesvh.cn/Article/details/ggzsltvjx.sHtML

[Q71] 查看建表语句
来源：http://read.share.zdbjq.cn/Article/details/gnunkrfne.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/gfmotmiyl.sHtML

[Q72] 查看索引
来源：http://3g.zdbjq.cn/Article/details/glrdxszzk.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fehbvm.com/Article/details/gqwhewatw.sHtML

[Q73] 查看表状态
来源：http://baike.fehbvm.com/Article/details/gvteymtmm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fehbvm.com/Article/details/giybdbruo.sHtML

[Q74] 强制使用索引
来源：http://3g.fehbvm.com/Article/details/gthgyryqt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/gedoodlkt.sHtML

[Q75] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gxoxzamql.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fehbvm.com/Article/details/gqjlycwfk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fehbvm.com/Article/details/gtwqihebt.sHtML

[Q76] 按天统计
来源：http://mobile.zdbjq.cn/Article/details/gjmigmjfz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fehbvm.com/Article/details/gzozwbrbj.sHtML

[Q77] 时间加减
来源：http://3g.hesvh.cn/Article/details/gmasyngfd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.zdbjq.cn/Article/details/gnebemxyw.sHtML

[Q78] 当前时间
来源：http://blog.fehbvm.com/Article/details/grnkehjrl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/gjujmcggm.sHtML

[Q79] 字符串拼接
来源：http://blog.fehbvm.com/Article/details/ghefmbrtj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fehbvm.com/Article/details/givfozjgi.sHtML

[Q80] 字符串截取
来源：http://wap.zdbjq.cn/Article/details/gpeeshvaq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gqhkrsigr.sHtML

[Q81] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/guinefwhs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fehbvm.com/Article/details/ggrzrvvsx.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fehbvm.com/Article/details/gurnannoe.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gcbdljsal.sHtML

[Q83] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gfhbhdlhx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gayuxeqzs.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/gscbwtpdb.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gnaxytzxw.sHtML

[Q85] 数值取整
来源：http://mobile.zdbjq.cn/Article/details/gqljjyybz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.zdbjq.cn/Article/details/gctrglzkq.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.hesvh.cn/Article/details/glwrknboo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.zdbjq.cn/Article/details/gpcndmhxg.sHtML

[Q87] JSON 字段做条件
来源：http://3g.hesvh.cn/Article/details/gbcinfxyv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.hesvh.cn/Article/details/gicroofmw.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fehbvm.com/Article/details/ghxvupehx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fehbvm.com/Article/details/gaqhxchbe.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.hesvh.cn/Article/details/guhaaukzh.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fehbvm.com/Article/details/gnzyhfwqy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gsssyzjab.sHtML

[Q90] 生成序号列
来源：http://blog.hesvh.cn/Article/details/gnngvzzzy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.zdbjq.cn/Article/details/gcuuosudb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grcqchrtn.sHtML

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/gmlidampx.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjdjprqxq.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fehbvm.com/Article/details/gexdphzdt.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fehbvm.com/Article/details/gzzgsscwp.sHtML

set -euo pipefail
来源：http://m.share.hesvh.cn/Article/details/gqlmovnpv.sHtML

[R02] 变量赋值与使用
来源：http://baike.hesvh.cn/Article/details/gfqqosfri.sHtML

name="Tom"; echo "$name"
来源：http://www.share.hesvh.cn/Article/details/gxltzsigy.sHtML

[R03] 只读变量
来源：http://blog.zdbjq.cn/Article/details/gecvxugfx.sHtML

readonly PI=3.14
来源：http://3g.fehbvm.com/Article/details/grrtnskxl.sHtML

[R04] 位置参数
来源：http://baike.hesvh.cn/Article/details/gvjuwpzfe.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fehbvm.com/Article/details/gmgsejkja.sHtML

[R05] 参数默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gegcikjzw.sHtML

name="${1:-default}"
来源：http://www.blog.zdbjq.cn/Article/details/gzqlcfvqe.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fehbvm.com/Article/details/gcccyalew.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gwlzpwwfw.sHtML

[R07] if 判断文件
来源：http://mobile.hesvh.cn/Article/details/gsoijldjo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gmfvjkkoo.sHtML

[R08] 数值比较
来源：http://3g.hesvh.cn/Article/details/goadfzqim.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/gdmraeiff.sHtML

[R09] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gyyhpveiy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.hesvh.cn/Article/details/gssjoeosk.sHtML

[R10] 正则匹配
来源：http://wap.hesvh.cn/Article/details/gmxpgkvxo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.zdbjq.cn/Article/details/gzxcrjtdt.sHtML

[R11] case 多分支
来源：http://read.share.zdbjq.cn/Article/details/gizmylmou.sHtML

case "$1" in
来源：http://m.share.hesvh.cn/Article/details/glsvhsjoo.sHtML

start) echo "启动" ;;
来源：http://www.share.zdbjq.cn/Article/details/gcrfggfwk.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/gumxnmorv.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/gecwbvwac.sHtML

esac
来源：http://www.m.share.hesvh.cn/Article/details/ggofcjnwb.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/ghzqhjolc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.zdbjq.cn/Article/details/gbpsphqyu.sHtML

[R13] for 计数循环
来源：http://www.blog.hesvh.cn/Article/details/gujvwtbvj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gcsrbdjzo.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/gbmsmevur.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gcphizkia.sHtML

[R15] while 逐行读文件
来源：http://m.share.fehbvm.com/Article/details/ggoobdidc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/gmuhbjiom.sHtML

[R16] until 等待条件
来源：http://3g.zdbjq.cn/Article/details/gheyfcwqs.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gtrnvcbyz.sHtML

[R17] 数组定义与取值
来源：http://read.share.hesvh.cn/Article/details/gqkrkpdbw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/gmevswlle.sHtML

[R18] 遍历数组
来源：http://m.share.zdbjq.cn/Article/details/glnxknsvf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fehbvm.com/Article/details/gibiozitm.sHtML

[R19] 数组长度
来源：http://3g.hesvh.cn/Article/details/gybaaiebz.sHtML

echo "${#arr[@]}"
来源：http://m.share.hesvh.cn/Article/details/gnayupzri.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.zdbjq.cn/Article/details/gzegnwvmj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.hesvh.cn/Article/details/gruyqziui.sHtML

[R21] 字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gpzrtklia.sHtML

echo "${#s}"
来源：http://www.blog.hesvh.cn/Article/details/gsalzjmjo.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gpqnjwzdc.sHtML

echo "${s:0:5}"
来源：http://3g.zdbjq.cn/Article/details/gpvfuokfs.sHtML

[R23] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gonsczeov.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.hesvh.cn/Article/details/ggvehckjo.sHtML

[R24] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gljbzwnsm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.zdbjq.cn/Article/details/grktwbnwv.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.zdbjq.cn/Article/details/gzpeibrno.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fehbvm.com/Article/details/gqxxtjvhw.sHtML

[R26] 命令替换
来源：http://wap.zdbjq.cn/Article/details/gvybbfpaa.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.zdbjq.cn/Article/details/glrqaoguu.sHtML

[R27] 算术展开
来源：http://m.share.fehbvm.com/Article/details/gobxkfwgj.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fehbvm.com/Article/details/gcaiwqgwn.sHtML

[R28] 浮点运算
来源：http://read.share.fehbvm.com/Article/details/gbhplcqbk.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.hesvh.cn/Article/details/gcdvyxqxo.sHtML

[R29] 定义函数
来源：http://m.share.zdbjq.cn/Article/details/glvcutzvl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.hesvh.cn/Article/details/gqmiidmvr.sHtML

[R30] 函数返回状态码
来源：http://3g.fehbvm.com/Article/details/girsgevta.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.zdbjq.cn/Article/details/gdntabswe.sHtML

[R31] 局部变量
来源：http://baike.hesvh.cn/Article/details/gavdtocjo.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/ghrixnzon.sHtML

[R32] 参数个数校验
来源：http://m.share.hesvh.cn/Article/details/ghidnwniy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gqkdtdinc.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/gpbvxfnue.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fehbvm.com/Article/details/gfjwduqiv.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/gebinmjyl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gzhdzjxye.sHtML

[R35] 后台执行并等待
来源：http://m.share.fehbvm.com/Article/details/gbzotfheh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fehbvm.com/Article/details/gimhwkhyx.sHtML

[R36] 并发执行多个任务
来源：http://m.share.zdbjq.cn/Article/details/gamciacep.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/goewtlzzw.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/glfyoopib.sHtML

files=$(ls -1)
来源：http://www.m.share.hesvh.cn/Article/details/gdjtikhii.sHtML

[R38] 管道串联
来源：http://blog.fehbvm.com/Article/details/gcypqysxj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fehbvm.com/Article/details/gjwreysdz.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fehbvm.com/Article/details/gcprtoall.sHtML

cmd > out.log 2>&1
来源：http://baike.fehbvm.com/Article/details/giosyldjg.sHtML

[R40] 追加写日志
来源：http://read.share.fehbvm.com/Article/details/gqdmvcbhi.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/gvjgqhqqr.sHtML

[R41] 丢弃输出
来源：http://mobile.zdbjq.cn/Article/details/gebowepgb.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gqkkhtfur.sHtML

[R42] 输入重定向
来源：http://wap.hesvh.cn/Article/details/gbpnshall.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/gyitmwure.sHtML

[R43] 按名字查找文件
来源：http://wap.zdbjq.cn/Article/details/gtebftjcc.sHtML

find . -name "*.log" -type f
来源：http://read.share.hesvh.cn/Article/details/gkxfesnwy.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/gdrpojltn.sHtML

find . -mtime -7 -type f
来源：http://read.share.hesvh.cn/Article/details/gfaqtracs.sHtML

[R45] 批量删除
来源：http://www.m.share.fehbvm.com/Article/details/geiyrahvg.sHtML

find . -name "*.tmp" -delete
来源：http://3g.zdbjq.cn/Article/details/gmasrzszb.sHtML

[R46] 递归替换文件内容
来源：http://m.share.hesvh.cn/Article/details/giyllejhu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.hesvh.cn/Article/details/gpgstocvz.sHtML

[R47] sed 单行替换
来源：http://mobile.hesvh.cn/Article/details/gwwziumwp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/gladhdtba.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gpcatwyec.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.hesvh.cn/Article/details/gvedhlyoz.sHtML

[R49] awk 带条件
来源：http://www.m.share.fehbvm.com/Article/details/gxpwiooto.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.zdbjq.cn/Article/details/gzmdajqgx.sHtML

[R50] awk 求和
来源：http://blog.hesvh.cn/Article/details/gwqqbkybe.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gpjitjbcu.sHtML

[R51] 排序去重取前几
来源：http://baike.fehbvm.com/Article/details/gvglfejai.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.hesvh.cn/Article/details/gnqmgycwm.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/grlptauhz.sHtML

wc -l a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gelevmtzy.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.zdbjq.cn/Article/details/gkkuvzctp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fehbvm.com/Article/details/giapsbkjj.sHtML

[R54] 比较两个文件
来源：http://read.share.hesvh.cn/Article/details/gohbzhiiv.sHtML

diff a.txt b.txt
来源：http://read.share.hesvh.cn/Article/details/ggytqrwva.sHtML

[R55] 压缩与解压
来源：http://baike.hesvh.cn/Article/details/gpyxzglxl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.hesvh.cn/Article/details/goacoopuv.sHtML

[R56] 远程拷贝
来源：http://3g.zdbjq.cn/Article/details/gjfsaepnj.sHtML

scp file user@host:/path/
来源：http://baike.hesvh.cn/Article/details/gduckvema.sHtML

[R57] 远程执行命令
来源：http://baike.fehbvm.com/Article/details/gbkomrebl.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.hesvh.cn/Article/details/giiisxmqq.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/gvqwdzluu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/gmvuxswab.sHtML

[R59] 发 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gvxglsvzs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/gancgebdg.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gfkzuzbiq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.hesvh.cn/Article/details/gwqiubypw.sHtML

[R61] 磁盘占用
来源：http://read.share.fehbvm.com/Article/details/gdeaewkew.sHtML

df -h;  du -sh *
来源：http://www.share.fehbvm.com/Article/details/ggkjhbyif.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/gigciomfg.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.hesvh.cn/Article/details/gfhxrhefv.sHtML

[R63] 内存与进程
来源：http://3g.zdbjq.cn/Article/details/guextgpix.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fehbvm.com/Article/details/gehpkwjzf.sHtML

[R64] 结束进程
来源：http://blog.fehbvm.com/Article/details/goxvxmnsf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fehbvm.com/Article/details/gssunltbl.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/gahrlpule.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.zdbjq.cn/Article/details/gnqdrfrqu.sHtML

[R66] 定时任务
来源：http://mobile.fehbvm.com/Article/details/gpdnzukfq.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/gswdwhutu.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.hesvh.cn/Article/details/gqzvuxnir.sHtML

openssl rand -hex 16
来源：http://mobile.zdbjq.cn/Article/details/gaywnfxku.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/gxqdreclq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.zdbjq.cn/Article/details/gektqrlum.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/gewdcrtgr.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/gketezwxy.sHtML

[R70] 时间戳与互转
来源：http://3g.zdbjq.cn/Article/details/gctfiqlwd.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.hesvh.cn/Article/details/gptyncanf.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gstgwtkkl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.zdbjq.cn/Article/details/goljlucdx.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/grwcgynnn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gskhfxhzd.sHtML

[R73] 分割大日志
来源：http://baike.hesvh.cn/Article/details/gwgddwaqg.sHtML

split -l 1000 big.log part_
来源：http://mobile.hesvh.cn/Article/details/gfanjkzzh.sHtML

[R74] 批量重命名
来源：http://read.share.fehbvm.com/Article/details/gudwpuluh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fehbvm.com/Article/details/gshxbnlit.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/gvftrosyb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.hesvh.cn/Article/details/gwesftqui.sHtML

[R76] 使用临时文件
来源：http://blog.hesvh.cn/Article/details/gxrfoeqgv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gsyqfcdci.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/gulkoxpkt.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/gxkeyxbtn.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/gnedgtekb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/gdhmbzffa.sHtML

[R79] 解析命令行选项
来源：http://m.share.fehbvm.com/Article/details/guaypbqel.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/gzdvufksd.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/gjqfdastv.sHtML

time ./run.sh
来源：http://m.share.fehbvm.com/Article/details/gxyckndmk.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxegrkbhn.sHtML

S. C / C++ 专题
来源：http://blog.fehbvm.com/Article/details/gtdrxudvd.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gzuazlelu.sHtML

[S01] C：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gdlcxtzxq.sHtML

#include <stdio.h>
来源：http://blog.hesvh.cn/Article/details/goejpfanz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.hesvh.cn/Article/details/gflqvvlqd.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/ganlflooy.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fehbvm.com/Article/details/gazmssyby.sHtML

[S03] C：读入整数
来源：http://blog.zdbjq.cn/Article/details/gclkxzkut.sHtML

int x; scanf("%d", &x);
来源：http://wap.zdbjq.cn/Article/details/grtpgtzxl.sHtML

[S04] C：字符串复制
来源：http://read.share.fehbvm.com/Article/details/ggwaozlyg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/ghtudcqfe.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gwhvcyskk.sHtML

strlen(s)
来源：http://www.share.zdbjq.cn/Article/details/gpiradzhp.sHtML

[S06] C：字符串比较
来源：http://read.share.fehbvm.com/Article/details/gnofhajwc.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gtpkgfzgs.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/gkrirwgtr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/glkgfihxw.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/gqmmwpgdu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/gekdlbsxl.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.zdbjq.cn/Article/details/giafjtkue.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.hesvh.cn/Article/details/gfwqnfwbq.sHtML

[S10] C：指针与解引用
来源：http://www.blog.hesvh.cn/Article/details/gpkpfktgq.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fehbvm.com/Article/details/grmknbecn.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gyoenbqkk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.zdbjq.cn/Article/details/gktxustwc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fehbvm.com/Article/details/gixxxwrrp.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/gtngiajok.sHtML

[S12] C：写文件
来源：http://baike.hesvh.cn/Article/details/gysnpdfdg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.hesvh.cn/Article/details/grjgxysug.sHtML

[S13] C：宏定义
来源：http://www.m.share.zdbjq.cn/Article/details/goqkpltnb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fehbvm.com/Article/details/gsdraxjyv.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gbqolhjjb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fehbvm.com/Article/details/gkxzmvlpd.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/gjjlkjsiv.sHtML

(double) a / b
来源：http://baike.fehbvm.com/Article/details/gymkyqqgn.sHtML

[S16] C：位操作置位
来源：http://blog.hesvh.cn/Article/details/gfbvpzikp.sHtML

x |= (1 << 3);
来源：http://baike.fehbvm.com/Article/details/gmsekryak.sHtML

[S17] C：安全拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gdtowfhzg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/goqcbkwne.sHtML

[S18] C：命令行参数
来源：http://read.share.fehbvm.com/Article/details/grtwazuxy.sHtML

int main(int argc, char **argv)
来源：http://mobile.hesvh.cn/Article/details/gercnbyjz.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/gihjflrcq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/ggpmzbpdq.sHtML

[S20] C：二分查找
来源：http://www.m.share.zdbjq.cn/Article/details/gnlyhvejt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gonbsdefb.sHtML

[S21] C：字符类别判断
来源：http://blog.zdbjq.cn/Article/details/gimexdgkv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.zdbjq.cn/Article/details/gjmepgcol.sHtML

[S22] C：字符串转数字
来源：http://3g.fehbvm.com/Article/details/gjfnfdaeo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fehbvm.com/Article/details/gstvahkli.sHtML

[S23] C：随机数
来源：http://read.share.hesvh.cn/Article/details/gkycmrcgs.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/gemtdfkic.sHtML

[S24] C：获取本地时间
来源：http://mobile.hesvh.cn/Article/details/gpueqcxyw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/goxennwsg.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/ghgeisjio.sHtML

memcpy(dst, src, n);
来源：http://www.share.zdbjq.cn/Article/details/guygpuspr.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/gohijrfkc.sHtML

memset(a, 0, sizeof a);
来源：http://baike.hesvh.cn/Article/details/ghdbqzxos.sHtML

[S27] C：定义常量
来源：http://wap.zdbjq.cn/Article/details/gzbttvvhd.sHtML

const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gacxolhlr.sHtML

[S28] C：静态变量
来源：http://baike.fehbvm.com/Article/details/gkqjohoum.sHtML

static int counter = 0;
来源：http://www.blog.hesvh.cn/Article/details/ghyhhhwiq.sHtML

[S29] C：变参函数
来源：http://www.m.share.hesvh.cn/Article/details/gwrwwzcte.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gljrdpmid.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gtawczjnn.sHtML

#ifndef X_H
来源：http://baike.fehbvm.com/Article/details/gzwwyboaq.sHtML

#define X_H
来源：http://www.share.fehbvm.com/Article/details/gluqwwuul.sHtML

#endif
来源：http://baike.fehbvm.com/Article/details/glmopvlrm.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/ggnxqroeq.sHtML


<!-- 参考信息 -->