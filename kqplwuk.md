代发 wailian999

[Q65] 回滚事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrdigkjx.sHtML

ROLLBACK;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtmokpiy.sHtML

[Q66] 行锁查询
来源：http://3g.fanxiaobao.xyz/Article/details/glewrngnp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fanxiaobao.xyz/Article/details/gvivmbfyp.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvykodfh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fanxiaobao.xyz/Article/details/gdwkontco.sHtML

[Q68] 保存点
来源：http://baike.fanxiaobao.xyz/Article/details/gflzexoee.sHtML

SAVEPOINT sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvrcaeiz.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/guiplaquj.sHtML

[Q69] 查看执行计划
来源：http://wap.fanxiaobao.xyz/Article/details/gzafzufuy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fanxiaobao.xyz/Article/details/gmpidhbgq.sHtML

[Q70] 更新统计信息
来源：http://wap.fanxiaobao.xyz/Article/details/gfpbsrfub.sHtML

ANALYZE TABLE users;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdwdwwbe.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fanxiaobao.xyz/Article/details/giunevqaf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsksllolr.sHtML

[Q72] 查看索引
来源：http://wap.fanxiaobao.xyz/Article/details/grfmzrnat.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzbgzcub.sHtML

[Q73] 查看表状态
来源：http://blog.fanxiaobao.xyz/Article/details/gpvuqqfwy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gfdvbjpbk.sHtML

[Q74] 强制使用索引
来源：http://www.share.fanxiaobao.xyz/Article/details/glgavfemb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavbhzfmj.sHtML

[Q75] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gioaxxolc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqntztbzd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/gashcsbhv.sHtML

[Q76] 按天统计
来源：http://3g.fanxiaobao.xyz/Article/details/gbyerrmfb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnegozrjy.sHtML

[Q77] 时间加减
来源：http://blog.fanxiaobao.xyz/Article/details/ghfixtjxc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fanxiaobao.xyz/Article/details/gdycevbdd.sHtML

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gnycolpfk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fanxiaobao.xyz/Article/details/gysufoyin.sHtML

[Q79] 字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/goukuxhqr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzpytjlg.sHtML

[Q80] 字符串截取
来源：http://www.share.fanxiaobao.xyz/Article/details/guxlvmcwv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/grajqoeml.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/ghcricqpy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkltvbuk.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fanxiaobao.xyz/Article/details/gdyayiikd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/giqcdaagy.sHtML

[Q83] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnhcqdrl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gyvvsvpcf.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/gycjkkdny.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gptrehult.sHtML

[Q85] 数值取整
来源：http://read.share.fanxiaobao.xyz/Article/details/guqtfnmmo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpykjdvcp.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/greppbuvx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqpbftax.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gnibouzce.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fanxiaobao.xyz/Article/details/gwufosgoi.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fanxiaobao.xyz/Article/details/grwjkccqt.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlmbjrqq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorjtllat.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdakqfwj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gubdyykij.sHtML

[Q90] 生成序号列
来源：http://wap.fanxiaobao.xyz/Article/details/gqkukeumx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhuzpprk.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/giuvuofak.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucnkdhrt.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvosggkp.sHtML

[R01] shebang 与严格模式
来源：http://blog.fanxiaobao.xyz/Article/details/gzgvvdyaa.sHtML

#!/usr/bin/env bash
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbridcry.sHtML

set -euo pipefail
来源：http://mobile.fanxiaobao.xyz/Article/details/gykvoiqxl.sHtML

[R02] 变量赋值与使用
来源：http://blog.fanxiaobao.xyz/Article/details/geyrutstk.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/glwegllco.sHtML

[R03] 只读变量
来源：http://blog.fanxiaobao.xyz/Article/details/gbvedftzl.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/gjtqsqtae.sHtML

[R04] 位置参数
来源：http://3g.fanxiaobao.xyz/Article/details/gkrruydkw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fanxiaobao.xyz/Article/details/gudilzjox.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmrgqxpt.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/gcttxehky.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpffhtlj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzixepagi.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gzyruawhc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/glodzzbhl.sHtML

[R08] 数值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/grrxgissr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gzffivcti.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdnhnmtt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/guogzopbh.sHtML

[R10] 正则匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzsuigew.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtsomrkzj.sHtML

[R11] case 多分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwzgpdeo.sHtML

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyohrlzkr.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gidvzuuar.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gwmdliwft.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gsjzhpjuc.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/gilrflkap.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsuefalx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/grpdmtmvp.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpthfejk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywmlezup.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/goigoikhd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gmyjykkew.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhtjtqnz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyavbqpb.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgoxzbwy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gonmfpacv.sHtML

[R17] 数组定义与取值
来源：http://baike.fanxiaobao.xyz/Article/details/gdriseznq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjwdnvwb.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gilyqqkgo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gtmomufgy.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/ggquxbfto.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gljayzwfv.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/goldhbjuo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnstpvjl.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtafpccc.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/gnmfajorx.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkibfhir.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/gusdtbgcz.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gmcgzuopg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/gmwmrjoer.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmicvotgo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gboulxhmc.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/guuxgupsk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gsjmeyzuf.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gqiffrxfd.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbaiccko.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gnbkybujx.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/gcxyungsm.sHtML

[R28] 浮点运算
来源：http://blog.fanxiaobao.xyz/Article/details/gxnfhhdiw.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpaxrhdm.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbzlzzhr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/gcweeosxk.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gtdwxvamj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcmnlimr.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxqjnadw.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbqfcadt.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmiwiwudt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gpgbsqshi.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gglwavwrj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/gygwillns.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gnfxbcbit.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gkliodoec.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gvkyhllpo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/glbvucoyb.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwoxbxnr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gukypqaht.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdcretjp.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljafuzti.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gpsqisktc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/grmahicyd.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/gjpdsfdoj.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgttonja.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/guuoavish.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gczffiwly.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/gsmokvvoj.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmmutjvg.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gtptzwqbk.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gxuueanki.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gsjztrchr.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gblejouzh.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geofydayz.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfejskwaz.sHtML

[R45] 批量删除
来源：http://m.share.fanxiaobao.xyz/Article/details/ghozdtrgs.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giarrosmm.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getehpjoa.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gircwxvxx.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/glslsuuai.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gayjrkiwd.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gwaldwrwr.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gauhfftbl.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gvaqefrqj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqcupgon.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpteuagmi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gczimtbic.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/gtegtwrdc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfeujctdg.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/glamhdgen.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddyhbifu.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gvkxnttxz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gwzbwklgs.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/glltleccp.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gvusdwvdn.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gysdncwyt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/goajnliui.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gdkzefwnj.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyiexwnel.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbgwndsa.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gehillyay.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxirhpkc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqejojdb.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfkymdod.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqwmxlox.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbbklrxh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gpqmtaiqa.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvlchlty.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gqmgorrds.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqkjsekn.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkzrlkde.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxlagykv.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/ginqnflvm.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxxrsxqb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmttkkss.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkhsfakh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gpktjrvho.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gvpivkehi.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvqwpptq.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gmceubocy.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gmoyjopwu.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbreyvhw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/glvethdaw.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/godfwwlaw.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/grqaebxph.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gqinxattt.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjakavxh.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsxkyshb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/gainokitn.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gngsljvze.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gmyzvlygj.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/geblqqwow.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljumpkeq.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzelcrpz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gulvjouky.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gtemhjime.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/geftgryvy.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gczixuqyd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/govgyjvta.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grshholcf.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqopmbqs.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gevbegyhi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsagwxbe.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvoqtirs.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdnfpxhu.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/guqhcttgf.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrbetkzd.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gxyqeryvg.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gttyiwkws.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gekujlrcq.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gdznwnrmo.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/genfnhojg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjiduqgkx.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/ghjugsxcd.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdkypkoy.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlbsnsrg.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/gmthhaihi.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gpqnprhwj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gvlkxoxpk.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gfbflsoda.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gocooxbrh.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gdyydkijz.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gwpydguje.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjphalmpf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gvwefpyut.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjwgirxq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgtntrie.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gfuubfbho.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjlylryq.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gmullwbpa.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gbnpgtycw.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcijpiwv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/grqvncbdc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gdwwmanjy.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihlrfewf.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gumblfkjs.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gjokmfzca.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gizpoxdqu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gcyzoyktm.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gqmelvajb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwfvaeck.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/ggnbelxhv.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/glmeausec.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/ginzelhla.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjyyrbxu.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gdrxsljnx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrxmpald.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gvncsgtom.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpocdwzq.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvilblzg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/geyonicqj.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxkuvvgx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gydrdvxcu.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/ghvrusbty.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvnkfvgr.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbwcdrrz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhubandx.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gylvagxsn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsggcbwxf.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurtlszgo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/gktlwgfit.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwgkyzzj.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdfujbpx.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/glqhmjhzv.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmbajhto.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/grxoptqea.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gxudtyzzm.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gddhzvfgk.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnkmhvei.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggaigpfww.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gcdqgmwpw.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gqbryttin.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdujqavd.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gdngjlidx.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtjppvhn.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxassogkt.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/growkslex.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gfvjkanzf.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqjgymhq.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlkgdfdg.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbopqgfj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwqcjnlb.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/gukoyrtgs.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/guypfxxbe.sHtML


<!-- 参考信息 -->