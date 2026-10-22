代发 wailian999

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2nylayfci.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2xibuvsev.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2dkhwoxvf.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2xpvzbruh.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2uwygojii.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2vipxrpev.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2ezeowbnp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2jlpqfjcj.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2zjeagury.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2avwijdez.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2aefxebah.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2yqosymau.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2oqozhifc.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2jrryzbhv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2elfwvgor.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2xjuydwhn.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2wnvfhbsv.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2izcxrotu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2jbdfubqc.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2jwavpkmh.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qgugrzyr.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2kpmteusf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2pavsekoq.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2voujembh.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2qtnkvklb.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2mlrclgwe.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2iqqtzmup.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2xxrfofvr.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2kxzqrtgn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2ldxcqobm.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2wkzyrcql.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2uawckwxn.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2lkcluebw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2ujgoykwg.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2dnvhamyq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2avlptvvo.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2ozmkiope.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nrfktilw.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2etiujsod.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rqnqxzzx.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2xmbyvkyp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2elypqcvp.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2gfidwnsg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2naqlvkcz.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2pxaozevl.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tvwkkvwr.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2mrddviqu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2hdqtbtxi.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2pdrpulom.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2ozvkigvk.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2eskvsvyd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2knjsryrd.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2pesphlnb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2ejqhejmi.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vwkeqlji.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2poplegyu.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2dscfmcoe.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2veqfzxdi.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2knaejvja.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2apwwirlw.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2szeimbzz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kllfxffo.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2cigdnpry.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2lsypmtix.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2tapqjuoj.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2ftxhsbbm.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2fveobgpi.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2sntweaec.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2ybmnomrz.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2wfnjmjif.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2fsaqnqcd.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2bfekzakd.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2wqtiqpln.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2lpbmclit.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2qyorqdeh.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2bvxjerte.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2tolfewmz.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ufprnyjb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ylbfganx.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2rozmipqz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2klbxceea.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2ohvtrhjo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2tdnwkkyd.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2hnxfbuzo.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2qicekvqg.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ajlswkhn.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2zxuvnwpm.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2htpnycum.html

esac
来源：http://www.52xcode.cn/Article/details/gt2lwnznmby.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2tocmdjcs.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2flkqkbqb.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2tygibkrj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2mischwfe.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2rwqkmwqr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ghbcpyea.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2hyynyinf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hnlzitio.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2rffmzaxg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ldzfvcoi.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2grwzkpzp.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2ftrkjraa.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2wociwhtm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2mbialtmr.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2zjtwhdia.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2ysxflcts.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2nwwfitrk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2arufchgj.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2yivkybzv.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2lykrtanz.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2meicggsq.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2fhdkvloy.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2izuvhnoa.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2vjcgpywy.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2xenmujkj.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2gnuhzwmi.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2xqpbwfqv.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2keloftxj.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2gihnwhei.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2elmwfaeb.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2lpigfrox.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2gxqjlbqc.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2yvtyurvr.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2adrlqmsf.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2gaxkubzz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2zuihndif.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2ybrbxtgs.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2lyrjzfkm.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2buitjgmf.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2lpzgqsei.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2uwgozakd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2bhoqiwim.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2kqnrchgd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2dgvjogmp.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2wadpjidx.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2adpdzxla.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2heuwfvmq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2mlkeatpo.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2yckeqzrk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2xcdscxyu.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2zedrcyuw.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2lmboijtt.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2jobtmzla.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2uldcephe.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2cvkuyzlu.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2omxtdyjp.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2pevummgs.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2cmrjtiap.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2rfsgsflx.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2fqtvshzy.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2xpqvjljh.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bbmxvpwx.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2ocibiwmv.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2wncnncbx.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2owobujqt.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2qdzasnzm.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2opixmsbr.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2frfnbvyb.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2muhkcxea.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2tendzpxm.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2nnomrtgb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2modztaaq.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2xaizqyta.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2plpfxxyg.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2qrtndyhw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2pdujtlin.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2moommork.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2lgpxuibj.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2ddrhqpuf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2capwtihs.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2ytwugdka.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2zgdqvovc.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2uplvhcia.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2zmbczunb.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ixpaxdwr.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2jgntslpe.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2icapziym.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2rzrgyhpi.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2tpizbbiu.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2bwgjvrpr.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2tkxxjfcg.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2yblfuhof.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2vhrnmszr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2kntuvrdh.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2fmorzhjv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2htwqcdfk.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2wyirakby.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2ovxukpgk.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2wslwysot.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2gzkeqjdr.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2wlqvpiqg.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2gitmovsp.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2cvzfofhe.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2sjzqdgii.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2gtlqvqgk.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2wrfszuff.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2dirdrsrf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2jsvvzwpj.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2hwrqbmau.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2sljrvvtr.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2emlpstqk.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2hrdbankk.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2oszrzyjo.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2kdijopgn.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2fhmtkjxo.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2sdkzyeoa.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2jbrrvcku.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2yjokxfyr.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2hshbrgzp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2fzljguoj.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2oxiizbgv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2edzsbsxd.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2notxizfi.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2pgimdkae.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2tfhmefdg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2mxkcoual.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2zsfrvuxv.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2lbwdgohd.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2cxvumjbd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ruelklzi.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2spwcvunt.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2hrhymzbx.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2cspqebbr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2cnhnytsr.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2xvaqajaj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2kassmhpx.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2zutxngfz.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2cwdalwnw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2obvnrzjv.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2jfwrplco.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nreivcyj.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2thcprbvo.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2yiiegqua.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2imsgrodv.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2zedwmplo.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2fzvdldag.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2jfnlujwr.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2phaejaan.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2afqicvak.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2pcpdsktu.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2pwzcatmi.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2paunfksb.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2crgwadnz.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2fyhygcmg.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2phkqbvky.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2wvcmybbx.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2tntqrele.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2pqrlbxwj.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2hdvqodrg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2sjvylbtk.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2dqlvdiwn.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2nswrmcem.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2bnyfwchs.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2aqnekjbc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2goycfwhy.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2gfydnvsv.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ccaglyxl.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2ibnlemko.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2rgbwxznv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2ldggcoov.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2phtezyzv.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2bsgdcgrj.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2yjtqcnke.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2ltgjhoej.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2jxaamvyn.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2uqeyrsgp.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2hlxnjeet.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2ozebodbv.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2fqjkcdeo.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2addupqff.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2scgradap.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2sjfdxpmj.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2wwtnynod.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2vspfqmdy.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2kfbwmxvz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2zmsnfvnn.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2blipzzlo.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2ussexltz.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2xqbnncll.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2nqxurole.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2kedfoudx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2molveilq.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2qppeqdaf.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2dmjwjjtn.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2zmddpplh.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2jqjiyewv.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2stdxeaco.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pfizbqbx.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2smdgjqab.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2olsdqhyv.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2kzsfwumu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2vykfmzyz.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2ciirmsje.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2sgdyzenj.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2eqqniryt.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2najvnyoa.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2smjkmwtp.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2hpdmeelh.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ywgmdytt.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hwtqizhn.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2kyagdqtm.html


<!-- 参考信息 -->