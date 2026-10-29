代发 wailian999

[Q63] 开启事务
来源：http://www.share.hesvh.cn/Article/details/gkovhpwro.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.hesvh.cn/Article/details/gwooetzuq.sHtML

[Q64] 提交事务
来源：http://wap.zdbjq.cn/Article/details/gsoormian.sHtML

COMMIT;
来源：http://3g.fehbvm.com/Article/details/gjeonvkqu.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/gtcuzozib.sHtML

ROLLBACK;
来源：http://baike.hesvh.cn/Article/details/grsylavap.sHtML

[Q66] 行锁查询
来源：http://blog.fehbvm.com/Article/details/gojlfukfq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.zdbjq.cn/Article/details/gtbiycpxy.sHtML

[Q67] 设置隔离级别
来源：http://wap.hesvh.cn/Article/details/gjhegrfac.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fehbvm.com/Article/details/gojeeingo.sHtML

[Q68] 保存点
来源：http://wap.fehbvm.com/Article/details/gcrslmzxl.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gmiqlujdm.sHtML

ROLLBACK TO sp1;
来源：http://baike.hesvh.cn/Article/details/ggaoklnsy.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/gegusttix.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.hesvh.cn/Article/details/gcffdcbql.sHtML

[Q70] 更新统计信息
来源：http://blog.zdbjq.cn/Article/details/gtiuaibkj.sHtML

ANALYZE TABLE users;
来源：http://mobile.hesvh.cn/Article/details/gvvhudrup.sHtML

[Q71] 查看建表语句
来源：http://www.share.hesvh.cn/Article/details/gxkqkbkcz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fehbvm.com/Article/details/gctgezxfk.sHtML

[Q72] 查看索引
来源：http://www.m.share.zdbjq.cn/Article/details/gljgxebzl.sHtML

SHOW INDEX FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gflelcwsw.sHtML

[Q73] 查看表状态
来源：http://wap.zdbjq.cn/Article/details/gpgjqbjiw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.hesvh.cn/Article/details/gngfsqfwz.sHtML

[Q74] 强制使用索引
来源：http://www.share.hesvh.cn/Article/details/gyhhlmkxa.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fehbvm.com/Article/details/gsbitmzkc.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gwbdelkgn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fehbvm.com/Article/details/guzfvqkwn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fehbvm.com/Article/details/gpdydyodj.sHtML

[Q76] 按天统计
来源：http://wap.zdbjq.cn/Article/details/gqtklbovk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.zdbjq.cn/Article/details/glgsnzsng.sHtML

[Q77] 时间加减
来源：http://m.share.hesvh.cn/Article/details/gtilnueqb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fehbvm.com/Article/details/ghfabxduk.sHtML

[Q78] 当前时间
来源：http://www.share.hesvh.cn/Article/details/gmktqrlba.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.hesvh.cn/Article/details/guvrxtsbg.sHtML

[Q79] 字符串拼接
来源：http://baike.hesvh.cn/Article/details/gavzdjqxi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.hesvh.cn/Article/details/ghmcupkjr.sHtML

[Q80] 字符串截取
来源：http://www.share.fehbvm.com/Article/details/gvclilqca.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gcwnrqgwf.sHtML

[Q81] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gwnugxzxl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fehbvm.com/Article/details/gcnlwaial.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.zdbjq.cn/Article/details/gilwluebu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gcnjcentj.sHtML

[Q83] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gcykgixvo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gvcpwufhc.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fehbvm.com/Article/details/giernsnqb.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/ghihvrmfe.sHtML

[Q85] 数值取整
来源：http://m.share.zdbjq.cn/Article/details/gqopjjtpg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fehbvm.com/Article/details/gcdeephvc.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fehbvm.com/Article/details/gocjxixag.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/ggjmdddzb.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fehbvm.com/Article/details/gmjnxosll.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fehbvm.com/Article/details/gaaphuydu.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/gjgkcjtrg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fehbvm.com/Article/details/gjomgkvzu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gzinghfjv.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fehbvm.com/Article/details/ggppcfmzn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.hesvh.cn/Article/details/gnvnrcxbo.sHtML

[Q90] 生成序号列
来源：http://wap.hesvh.cn/Article/details/goeaguiwp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fehbvm.com/Article/details/ghtgzfbqn.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gortqqtzz.sHtML

R. Bash 专题
来源：http://read.share.zdbjq.cn/Article/details/glrzvtlku.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxzyjqadk.sHtML

[R01] shebang 与严格模式
来源：http://3g.zdbjq.cn/Article/details/glvakzxqq.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/gkwllmpob.sHtML

set -euo pipefail
来源：http://www.m.share.zdbjq.cn/Article/details/gawbzaawm.sHtML

[R02] 变量赋值与使用
来源：http://baike.hesvh.cn/Article/details/gipwjvsxi.sHtML

name="Tom"; echo "$name"
来源：http://3g.hesvh.cn/Article/details/grbwklpjo.sHtML

[R03] 只读变量
来源：http://blog.fehbvm.com/Article/details/gtzokanng.sHtML

readonly PI=3.14
来源：http://www.share.fehbvm.com/Article/details/gnlbqvolb.sHtML

[R04] 位置参数
来源：http://www.blog.hesvh.cn/Article/details/gcfdceous.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.zdbjq.cn/Article/details/gybwoybjv.sHtML

[R05] 参数默认值
来源：http://www.share.zdbjq.cn/Article/details/gwucerkso.sHtML

name="${1:-default}"
来源：http://baike.fehbvm.com/Article/details/gqhpginzx.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/gpwfqqqdd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gppdyqbvx.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/gnlfocpom.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.zdbjq.cn/Article/details/gtlmeeexz.sHtML

[R08] 数值比较
来源：http://www.share.hesvh.cn/Article/details/gsjjvzqyg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fehbvm.com/Article/details/gxseykiqc.sHtML

[R09] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/gisvtpbjf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.hesvh.cn/Article/details/gocnxwzqk.sHtML

[R10] 正则匹配
来源：http://www.m.share.fehbvm.com/Article/details/ggpmnwroz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fehbvm.com/Article/details/gavuoodqv.sHtML

[R11] case 多分支
来源：http://www.m.share.zdbjq.cn/Article/details/gpctxkmmp.sHtML

case "$1" in
来源：http://www.blog.fehbvm.com/Article/details/grhiqwfot.sHtML

start) echo "启动" ;;
来源：http://m.share.fehbvm.com/Article/details/gslpuqzze.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gbtleqnrp.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fehbvm.com/Article/details/gyhxthpnh.sHtML

esac
来源：http://wap.hesvh.cn/Article/details/gepbotwbh.sHtML

[R12] for 遍历文件
来源：http://3g.zdbjq.cn/Article/details/gbqqmkvbv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.zdbjq.cn/Article/details/gvxglordu.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gwwfxfuuk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/ghuwpzaet.sHtML

[R14] C 风格 for
来源：http://baike.fehbvm.com/Article/details/gepnovcoz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gmquyicia.sHtML

[R15] while 逐行读文件
来源：http://m.share.hesvh.cn/Article/details/glndcxdxi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.hesvh.cn/Article/details/gmgywpkcd.sHtML

[R16] until 等待条件
来源：http://baike.zdbjq.cn/Article/details/gptvpvgsl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gwimxhjce.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/gggqkoogf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.zdbjq.cn/Article/details/gkagvkeye.sHtML

[R18] 遍历数组
来源：http://m.share.fehbvm.com/Article/details/gbrylicyv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.hesvh.cn/Article/details/gqxcbcyic.sHtML

[R19] 数组长度
来源：http://3g.fehbvm.com/Article/details/gkvuaiwjb.sHtML

echo "${#arr[@]}"
来源：http://baike.hesvh.cn/Article/details/gfmrurkif.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/gadgwprbb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.hesvh.cn/Article/details/gzycmdhzq.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/guezfjnxv.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/gbhodevkx.sHtML

[R22] 截取子串
来源：http://www.share.hesvh.cn/Article/details/genhajrmw.sHtML

echo "${s:0:5}"
来源：http://www.blog.zdbjq.cn/Article/details/grlpvxznc.sHtML

[R23] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gjevgzgzn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.hesvh.cn/Article/details/ggourkccy.sHtML

[R24] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gfphfonxs.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fehbvm.com/Article/details/gjjkabskg.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gsoykhfix.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.zdbjq.cn/Article/details/gipvwrhoj.sHtML

[R26] 命令替换
来源：http://m.share.hesvh.cn/Article/details/gkrfxghha.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fehbvm.com/Article/details/gllncmjnc.sHtML

[R27] 算术展开
来源：http://3g.zdbjq.cn/Article/details/gynxvifav.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/gandgigrc.sHtML

[R28] 浮点运算
来源：http://www.share.hesvh.cn/Article/details/gzzmkhouy.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fehbvm.com/Article/details/gcizsguci.sHtML

[R29] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gdxslpqel.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.hesvh.cn/Article/details/gbzbzkdss.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fehbvm.com/Article/details/gcpcvnxfa.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fehbvm.com/Article/details/gphcirxyu.sHtML

[R31] 局部变量
来源：http://3g.zdbjq.cn/Article/details/gfjjlltjy.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.hesvh.cn/Article/details/gvyncgyxy.sHtML

[R32] 参数个数校验
来源：http://wap.zdbjq.cn/Article/details/grizetysg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gbkgtiird.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.zdbjq.cn/Article/details/gioixhqzj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.hesvh.cn/Article/details/gnahmhzhm.sHtML

[R34] 退出时清理
来源：http://m.share.zdbjq.cn/Article/details/ganqxreok.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/grocsbrfy.sHtML

[R35] 后台执行并等待
来源：http://blog.fehbvm.com/Article/details/gtqwlfagu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fehbvm.com/Article/details/glidjfllf.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.zdbjq.cn/Article/details/gyrnlwfcx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fehbvm.com/Article/details/gqpqjiopu.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fehbvm.com/Article/details/gzabspblx.sHtML

files=$(ls -1)
来源：http://blog.hesvh.cn/Article/details/gxjwanzrq.sHtML

[R38] 管道串联
来源：http://www.blog.hesvh.cn/Article/details/guijsamjd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fehbvm.com/Article/details/grhjoixls.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fehbvm.com/Article/details/gaajjkupx.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gsrufcswg.sHtML

[R40] 追加写日志
来源：http://blog.zdbjq.cn/Article/details/gwizxpzbi.sHtML

echo "log" >> out.log
来源：http://mobile.fehbvm.com/Article/details/gvbszryfo.sHtML

[R41] 丢弃输出
来源：http://baike.zdbjq.cn/Article/details/gawpugvyg.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.hesvh.cn/Article/details/gysfiunli.sHtML

[R42] 输入重定向
来源：http://mobile.hesvh.cn/Article/details/gsswktnbh.sHtML

wc -l < a.txt
来源：http://www.share.hesvh.cn/Article/details/gitbvrowh.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fehbvm.com/Article/details/gwsoljgpj.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/gkqtdloge.sHtML

[R44] 按修改时间查找
来源：http://www.blog.zdbjq.cn/Article/details/gcpshqzdi.sHtML

find . -mtime -7 -type f
来源：http://baike.fehbvm.com/Article/details/gvtihjoqz.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/gvqfqfvba.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.zdbjq.cn/Article/details/glnrnhoxt.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/gbodozydu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.hesvh.cn/Article/details/getveyemg.sHtML

[R47] sed 单行替换
来源：http://mobile.fehbvm.com/Article/details/gxcuwtieg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gmcuwlzjy.sHtML

[R48] awk 取指定列
来源：http://m.share.zdbjq.cn/Article/details/gvblwyacc.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gnucaqmuf.sHtML

[R49] awk 带条件
来源：http://m.share.zdbjq.cn/Article/details/geidxwjbq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/gufhgglal.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/gcbqturdh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gmnihiofc.sHtML

[R51] 排序去重取前几
来源：http://www.share.fehbvm.com/Article/details/gwrzyownr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fehbvm.com/Article/details/gtdydqhyy.sHtML

[R52] 统计行数
来源：http://wap.zdbjq.cn/Article/details/gomxdpqym.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/gwhxcoquv.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.hesvh.cn/Article/details/gzxhgedhl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.hesvh.cn/Article/details/gqnxxosxt.sHtML

[R54] 比较两个文件
来源：http://www.blog.fehbvm.com/Article/details/grfibfwhh.sHtML

diff a.txt b.txt
来源：http://www.blog.zdbjq.cn/Article/details/geupsbysn.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/gqakhfrqg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.hesvh.cn/Article/details/ggqbkaqnc.sHtML

[R56] 远程拷贝
来源：http://baike.hesvh.cn/Article/details/gwjfkfmdb.sHtML

scp file user@host:/path/
来源：http://wap.fehbvm.com/Article/details/glshvecct.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/gwaealwvo.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/ggciffftz.sHtML

[R58] 下载文件
来源：http://wap.fehbvm.com/Article/details/glxgcorxh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.hesvh.cn/Article/details/gawczcxhr.sHtML

[R59] 发 POST JSON
来源：http://m.share.hesvh.cn/Article/details/grzvobwva.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/gaphdidqy.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gtlewvgzw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fehbvm.com/Article/details/gjqzsfzlv.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fehbvm.com/Article/details/grxfgogyt.sHtML

df -h;  du -sh *
来源：http://blog.zdbjq.cn/Article/details/gnbkgkzyb.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fehbvm.com/Article/details/ghvvruemb.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.zdbjq.cn/Article/details/giqafxnma.sHtML

[R63] 内存与进程
来源：http://www.share.zdbjq.cn/Article/details/gtmdcbeat.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.zdbjq.cn/Article/details/glnuifrfl.sHtML

[R64] 结束进程
来源：http://wap.hesvh.cn/Article/details/gjdzczoru.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/gcnpvzrom.sHtML

[R65] 查看端口占用
来源：http://mobile.zdbjq.cn/Article/details/gvhduxsxe.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/gtvtxvynf.sHtML

[R66] 定时任务
来源：http://3g.zdbjq.cn/Article/details/gpzyfhfhw.sHtML

crontab -e;  crontab -l
来源：http://wap.fehbvm.com/Article/details/gowsulczo.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/giyripflb.sHtML

openssl rand -hex 16
来源：http://m.share.hesvh.cn/Article/details/gooyjgghp.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/gdoetufsk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/grddopnwk.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/gvptfffvx.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/gnpujdifo.sHtML

[R70] 时间戳与互转
来源：http://www.share.hesvh.cn/Article/details/gxyuubdjl.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.zdbjq.cn/Article/details/ggkamoaxx.sHtML

[R71] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gjbbzikya.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.hesvh.cn/Article/details/gfmsgmwwi.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/gfpskidcf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gqmfpiyay.sHtML

[R73] 分割大日志
来源：http://m.share.hesvh.cn/Article/details/gufjddtcn.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/gtwnndggv.sHtML

[R74] 批量重命名
来源：http://www.m.share.zdbjq.cn/Article/details/gykpocgle.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/goohfrpuo.sHtML

[R75] 导出环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gbklxgwwz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fehbvm.com/Article/details/geveefgbi.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/gpvzzgrmp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gvtypmmnb.sHtML

[R77] 读取用户输入
来源：http://blog.zdbjq.cn/Article/details/gqmrkmzbt.sHtML

read -rp "请输入: " ans
来源：http://www.share.zdbjq.cn/Article/details/ggvaplofc.sHtML

[R78] 交互式菜单
来源：http://read.share.hesvh.cn/Article/details/gjdcserjo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.zdbjq.cn/Article/details/glrzwznqy.sHtML

[R79] 解析命令行选项
来源：http://wap.zdbjq.cn/Article/details/gwnevybws.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.hesvh.cn/Article/details/guzkuveco.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.zdbjq.cn/Article/details/guoaytnwt.sHtML

time ./run.sh
来源：http://read.share.hesvh.cn/Article/details/gcgrrfvel.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjogldizy.sHtML

S. C / C++ 专题
来源：http://wap.fehbvm.com/Article/details/gyhwhhqoc.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqsohjsvb.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/glvpjpilq.sHtML

#include <stdio.h>
来源：http://blog.zdbjq.cn/Article/details/gqpnrpdku.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fehbvm.com/Article/details/gstpnvoge.sHtML

[S02] C：变量与格式化输出
来源：http://3g.zdbjq.cn/Article/details/gyhjjfifk.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.hesvh.cn/Article/details/gmafppcje.sHtML

[S03] C：读入整数
来源：http://read.share.hesvh.cn/Article/details/gwkoovttf.sHtML

int x; scanf("%d", &x);
来源：http://blog.hesvh.cn/Article/details/gvpprlbma.sHtML

[S04] C：字符串复制
来源：http://www.blog.zdbjq.cn/Article/details/gsdjowgey.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fehbvm.com/Article/details/gixgkzqfp.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gkadnzhnc.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/geyyaujem.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/gntxigkvn.sHtML

strcmp(a, b) == 0
来源：http://read.share.hesvh.cn/Article/details/gaauhyocg.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.hesvh.cn/Article/details/gsslkfocs.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.zdbjq.cn/Article/details/gyysuacba.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.hesvh.cn/Article/details/gzzwnnebr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/glmekbphy.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/gvbsyjoep.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/gaonlppna.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.zdbjq.cn/Article/details/glnylbeco.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/ghjdibipj.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gttsrmbrx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.zdbjq.cn/Article/details/gagqhjtuq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/guktqanws.sHtML

fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gdzgfpjwx.sHtML

[S12] C：写文件
来源：http://www.share.zdbjq.cn/Article/details/gpbnfrbcm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gvxveylsz.sHtML

[S13] C：宏定义
来源：http://blog.fehbvm.com/Article/details/ghabsyokp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fehbvm.com/Article/details/gjpagatpa.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/gjzkyshsc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.hesvh.cn/Article/details/gpwbtaejt.sHtML

[S15] C：类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gsfapsqdx.sHtML

(double) a / b
来源：http://www.blog.fehbvm.com/Article/details/gwwddirwv.sHtML

[S16] C：位操作置位
来源：http://3g.hesvh.cn/Article/details/gqpkotjub.sHtML

x |= (1 << 3);
来源：http://m.share.hesvh.cn/Article/details/gasjsubyg.sHtML

[S17] C：安全拼接字符串
来源：http://blog.zdbjq.cn/Article/details/grcdcggju.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fehbvm.com/Article/details/gkrokoghn.sHtML

[S18] C：命令行参数
来源：http://m.share.hesvh.cn/Article/details/ghuowvgpk.sHtML

int main(int argc, char **argv)
来源：http://blog.zdbjq.cn/Article/details/gemfhstpz.sHtML

[S19] C：快速排序
来源：http://3g.hesvh.cn/Article/details/gwufxupqa.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gfkdqavdi.sHtML

[S20] C：二分查找
来源：http://3g.zdbjq.cn/Article/details/gukdzefhe.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/ggjxjxtki.sHtML

[S21] C：字符类别判断
来源：http://baike.hesvh.cn/Article/details/gkfdgmqei.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.hesvh.cn/Article/details/gztesvmik.sHtML

[S22] C：字符串转数字
来源：http://www.share.hesvh.cn/Article/details/gibhghrlh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.hesvh.cn/Article/details/gltwabcud.sHtML

[S23] C：随机数
来源：http://www.share.hesvh.cn/Article/details/gtxsmxbqk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.zdbjq.cn/Article/details/gcuklrogi.sHtML

[S24] C：获取本地时间
来源：http://read.share.zdbjq.cn/Article/details/gknnuwrnx.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/gbjpiqvge.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/gnvqkzwci.sHtML

memcpy(dst, src, n);
来源：http://3g.zdbjq.cn/Article/details/gbqjoyidn.sHtML

[S26] C：内存清零
来源：http://baike.hesvh.cn/Article/details/grcsmlhxo.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.zdbjq.cn/Article/details/gybqpthhm.sHtML

[S27] C：定义常量
来源：http://wap.zdbjq.cn/Article/details/gxcbmddfm.sHtML

const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gdclnfwfc.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/gmuemyivt.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/glykwxbsw.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/ggplktdct.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/gandcjeoo.sHtML

[S30] C：头文件保护
来源：http://mobile.zdbjq.cn/Article/details/galxtuejk.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/gnpdtadfx.sHtML

#define X_H
来源：http://mobile.zdbjq.cn/Article/details/gkxdwpzbb.sHtML

#endif
来源：http://m.share.zdbjq.cn/Article/details/giztllcsy.sHtML

[S31] C++：Hello World
来源：http://blog.hesvh.cn/Article/details/giibkhbmq.sHtML

#include <iostream>
来源：http://wap.zdbjq.cn/Article/details/gxmxtplid.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fehbvm.com/Article/details/guzbllsqi.sHtML

[S32] C++：字符串
来源：http://www.blog.zdbjq.cn/Article/details/gjxkbpshn.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.zdbjq.cn/Article/details/gmbvermli.sHtML


<!-- 参考信息 -->