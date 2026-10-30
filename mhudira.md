代发 wailian999

[Q67] 设置隔离级别
来源：http://3g.fanxiaobao.xyz/Article/details/gvesrnjul.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbzpuicq.sHtML

[Q68] 保存点
来源：http://baike.fanxiaobao.xyz/Article/details/gxaseibhk.sHtML

SAVEPOINT sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gqyskvytt.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfgsdusn.sHtML

[Q69] 查看执行计划
来源：http://www.share.fanxiaobao.xyz/Article/details/gurvrltlh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxigtmfa.sHtML

[Q70] 更新统计信息
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbfvcazb.sHtML

ANALYZE TABLE users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmhxkkfh.sHtML

[Q71] 查看建表语句
来源：http://www.share.fanxiaobao.xyz/Article/details/gjotlxlza.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/gtogvhdrm.sHtML

[Q72] 查看索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxhmcqoc.sHtML

SHOW INDEX FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gllfxqhmq.sHtML

[Q73] 查看表状态
来源：http://wap.fanxiaobao.xyz/Article/details/ghgyhszpz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaylgidxo.sHtML

[Q74] 强制使用索引
来源：http://read.share.fanxiaobao.xyz/Article/details/geavnokjb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fanxiaobao.xyz/Article/details/gogspcybk.sHtML

[Q75] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gybbdmqdj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gkqwedxqk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihibwhrh.sHtML

[Q76] 按天统计
来源：http://wap.fanxiaobao.xyz/Article/details/glozvixtb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/gwmplloqa.sHtML

[Q77] 时间加减
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrqvyqki.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvnfrjqm.sHtML

[Q78] 当前时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowstoiia.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fanxiaobao.xyz/Article/details/glqapwskq.sHtML

[Q79] 字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gqgfyiueh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fanxiaobao.xyz/Article/details/gtptgikuq.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzghvkfmh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfmcmpos.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnoyngxug.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwpryzrg.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywyzhluq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtvsoxpx.sHtML

[Q83] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/guqqmakvc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzleyfwai.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/glgomnykc.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxahpbjyx.sHtML

[Q85] 数值取整
来源：http://m.share.fanxiaobao.xyz/Article/details/gzchjivqv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpethnvg.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fanxiaobao.xyz/Article/details/gboyrtthd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvuhdecrc.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fanxiaobao.xyz/Article/details/grzpslbie.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fanxiaobao.xyz/Article/details/gczgmnbok.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fanxiaobao.xyz/Article/details/gmkjgerbw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fanxiaobao.xyz/Article/details/gmwehuhwd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnoltykga.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gojkupoml.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gkeevgjfe.sHtML

[Q90] 生成序号列
来源：http://m.share.fanxiaobao.xyz/Article/details/gihabxprt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/grrlmlcwx.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gkrredntw.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcdimpgx.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gwfzabmpg.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fanxiaobao.xyz/Article/details/gguvbnoka.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/gbknhzznc.sHtML

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/gplmsrnzx.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/gqxnhhsoj.sHtML

name="Tom"; echo "$name"
来源：http://3g.fanxiaobao.xyz/Article/details/gxbgadcyw.sHtML

[R03] 只读变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwfjzlcm.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwmbavjy.sHtML

[R04] 位置参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtobpaxgw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fanxiaobao.xyz/Article/details/gebeiwaff.sHtML

[R05] 参数默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gcckohrna.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/glseyuoeg.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmlxdfcy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghbbrzylj.sHtML

[R07] if 判断文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpxcrlou.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gfsbmknar.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gfakjwstn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gezmcdfwo.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gzjzszwwg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbxqendm.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gfpouyogh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdhqhtsc.sHtML

[R11] case 多分支
来源：http://baike.fanxiaobao.xyz/Article/details/gihxxyjzp.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gjllnxhgp.sHtML

start) echo "启动" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gplzrirvx.sHtML

stop)  echo "停止" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gnwiodlgq.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwsvsljh.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/gudgdyxzn.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gymmkqcgk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfnufoao.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/grgzzvbpa.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmezmsnv.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/gnlekhook.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gboiamyju.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvprnrjn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gguticzql.sHtML

[R16] until 等待条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsljmdno.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gxaprgrlz.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfmgrlpr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/ghvqvbwcs.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/gqmmdiypy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpuptuavu.sHtML

[R19] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godlpwrll.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqiunfteu.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/grtkrsezf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gubrbcpok.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gpqpxkayq.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gobkwrnpp.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gdkgoejqe.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkplfcot.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gfmrchshd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gziitmyyq.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gamuakuik.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdspenlg.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/gtwtndbcd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlnwbquy.sHtML

[R26] 命令替换
来源：http://3g.fanxiaobao.xyz/Article/details/gsegctnvv.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/gxrfxosqq.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/garpgwkum.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gusphevru.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gmoepbogx.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gaolkgzud.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gnarnxtob.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/goapwbxev.sHtML

[R30] 函数返回状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gyykvbkyo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqpcuznk.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gbiixhxwk.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpxgkvop.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzagzhph.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/guvpnkewp.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gshxkrhak.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gegegborj.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgaqpjzc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gftlcufnc.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gqzgjcedd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gzryjksel.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmehfbhd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwufajcsj.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppoorcfs.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gidiolwoh.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/gevsvujgv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqedauar.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/ghgyjejqp.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbbnvibt.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzyazzbg.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gdvpmfsgw.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gakeavubs.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gzucqilsh.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/gxioztwxj.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gotppfxzz.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdexvvejj.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gcelchkey.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/ghztzkwdt.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpcvhzta.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidnsenvl.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gtspnslmg.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glesgvbrs.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/glgwhrnmd.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gbyrmemxl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gsrfmkpge.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gllemrahu.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgjxftbl.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjgcfkyb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbfbqfwh.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gaipzcjkp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjmvyeya.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykffgqlq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/gdffbtzco.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwkjdfti.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gomujdrar.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjzmuqfi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzsvlyer.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbawktvl.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gajqytgmf.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gybbnodjm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gawloucpw.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdcqsjus.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gzdoeesyy.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/gzmefowzu.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goopgaffx.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdvgfcwo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gcvoohulv.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzpelmbr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/guhfiadff.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gtifccdgq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gxjcfadyi.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/ggdvfuglb.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gitnjspvq.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gavnnsoqr.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grktthqna.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/geuouiyps.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gqichvonc.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gphqvrgsw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gzswkhncu.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gisxqwpqh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqbgnjhr.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gbclstbzs.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/gjorwheup.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gclkgkdig.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gycdremht.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtdjsezv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gmglwdxxr.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gttarxpia.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmivpanf.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gommymjdb.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gqutqwtwe.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gdokznpsv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gnhutptml.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/ghvzdnyiu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/glaxzbwjz.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumsvditu.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gyuthtbdx.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/gikkcexsb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gyhldrtyy.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gcowvosag.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/guzxxshpa.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhxqbzev.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrldayjs.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxidamnw.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdexdkwb.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/guvaqbrqc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gqvemrbcg.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmsqdjba.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonvwkksw.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/gmcpedrxd.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gouryaruq.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqhrzdmz.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/grhfztrun.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gcacwlonm.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gifqfyrnh.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gzuxkzlod.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/gwpezmgpc.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gndhotopi.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsuwyaemx.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gqowoyoid.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/gqgnrypvw.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gvoympdfj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gtmqthkqp.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdowvcxh.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqdkmcyl.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gcgxzdkjm.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqxfomjx.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmnvkggy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxrvfksd.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjcpfqgt.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guphtcmaf.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gvaypipqt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/ggxhkxnkr.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/giptremky.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwbhnunf.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnzoxdfd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapihnonw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gerqkhjms.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhgcxacz.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvegezyg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gjbzyqnac.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/gptfpboqa.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrdemmdv.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcutilia.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrqitivl.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gshgmtuha.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gawmphupf.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gxyityjiv.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzyopftn.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gkvqlesqr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gerblgvcc.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzozxvbfi.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzomxaqo.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gltbaitrs.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcluqbdtj.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/ghlxhwiql.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gfwbkkmoo.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gppnwbduj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbryalvly.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gfevxqnvs.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzusqjtra.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktqjfsdl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gnfyymhcr.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gfljwvfir.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztivropo.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gffkmgeje.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gqnnscffv.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/gdzuhfpzm.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcprnhfeb.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfwtddla.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gkgcptlzz.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gkppksiop.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gazrdlnww.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/guedmzyox.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gweovyhvy.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gbugkspyz.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkzlvvjz.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gyikxvfli.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwsohmct.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgfsysuz.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbopxenz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpeugnsyw.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/grvmmfbnl.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/glhellxfr.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/grldkjnvg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gusfpmgxb.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gdxweiuyw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxspcsdtm.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gjtkhurjj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazzcmakw.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gogqdtpde.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssywhmkv.sHtML


<!-- 参考信息 -->