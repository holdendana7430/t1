代发 wailian999

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3aqokrean.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3wwgkhabo.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3oegtntao.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3hjqlgcfe.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3qntwgcwu.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3ikmlrhrs.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3zblexrky.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3wmalepqj.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3gfkppadx.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3shabjbyk.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3vlmdnpfi.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3bbdctqoz.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jskjrlaw.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3dzhqrvlk.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3wbnhmgmm.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3qijjxmxr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3omhwzjuq.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3qddklbez.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wikxktin.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3qaagvotd.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3bvrujvop.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3ksfnbmgs.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3wgxmsbwq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3yxlhnkow.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3hykikwbm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3ihnwdfxt.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3xcblktps.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3gihujyic.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3fpdumvfl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3inxazgwc.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ndhgortx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eopybllp.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3ciktdabj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cjozqhyd.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3aiuzzgho.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iyvmggeb.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3kojsrmtu.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ojladzjc.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3ucermmat.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3eeiyhdoq.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3bqftpyab.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3bisbhcfp.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3mlnqezlo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3ywntbbld.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3dtzdjqow.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3zappyvqz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dzhkvyqz.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3wuoghiya.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3lpqslwlp.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3xkqculuo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3ogioewuu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rzifooji.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3bhsayyhd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eimieqwm.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3bksgdivv.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3fmwhldhc.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3svkncaqq.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3izyisjvk.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3nejxdgpz.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3xmeiqgbm.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3mrvkpwll.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3fllhkjmw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3gupbcnky.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3mhmfbvwt.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3zodedrbb.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3ltdikdpg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3lskmrkfk.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3lkrmzgsy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3xyjyfige.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3oipsfvmh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3flvmvdoy.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3kykrlpfm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3sbgpztkp.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3oltnqxqj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3rvgjohyp.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3cecxyhfb.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3fxaldmqi.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3tthnhuaq.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3irmjtgdb.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3feigqsof.html

esac
来源：http://www.52xcode.cn/Article/details/gt3wtmnjjhs.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3gdylttju.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3cbwvgxmt.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3rqxyqjnt.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3feuhtfod.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3sghladyz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3sexqnjbo.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3dbxrrgri.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3xchsoogw.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3wrhzklmr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3yyrxxoes.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3xhrzclyz.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3xrgytqby.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3slcgxoqf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3invgyjyp.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3jxxgzgqh.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3anfqaesp.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3cqhgalek.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3cpumzquh.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3oljcoaty.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3nwpynbjz.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3pwlqcapr.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3dciphyap.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3biasiuvb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3xbeatnxr.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3jdapvlud.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3adyrdopx.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3dfurqkyl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3orgwalxm.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3zeowwimx.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3dunkwwrx.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3gniignss.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3xchybqsg.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3ybvjirtl.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3heoaesol.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3nfwoxhff.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3xonmzhcd.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3eqclgrdv.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3jiywdooj.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3wozynmgz.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3lryatkkp.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3hugvvsnr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ktjgyinw.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3tavovbmw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3mhxbkqnl.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3ctkkbetj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ooebyuwg.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3blvtlvmp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3svhpjzuc.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3dccglbzp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3plzikrge.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3pftojjrw.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3zkguhhth.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3jdwpuxgo.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3fypaueap.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3ctwvtyvg.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3hvsjtmzn.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3lyvjewrk.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3kbpkvgmw.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3kggwlgzf.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3igbsvhld.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3crpmrrxq.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3ygewwbqc.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3zwqiytae.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3azvppzuu.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3ffylufku.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3tosndsmu.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3ntnlbhkn.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3nppdagsb.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3gtjrduep.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3lgwrzvcv.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3cojwmngv.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cpvtgfzh.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3dzlnzveh.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dfuzbsay.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3npqpsnga.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3ppxtghcb.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3awpxrppe.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3wmxcacax.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3mmmfzkbo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3vbzufbnv.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3lesiuqfx.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3usaghuyd.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3ogudrymq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3czlzeyoj.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3mbtvfjwe.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dqznlich.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3cphoqjjv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3stfivkep.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3kdbrdmol.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3ipbzjxrk.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3bxfbxpkh.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3rnvwvwuo.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3rlfmaqra.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3dxfbywqk.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3wxgcrymi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3nsanuoce.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3dmfffric.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3yjgjxdhu.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3wuhaydoo.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3hvxhpcay.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3oqatiobm.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3gwdjrawj.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3nsjnxxxs.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3sfgrwuer.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3xvedzoxn.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3sxxfzqfy.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3idedzkpr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3rtvntaxm.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3vbigohuu.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3psirgdjs.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3uoljbkcp.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3dzkbzomc.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3mxnydavf.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rmlyzjco.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3bqdwougp.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3mkcpebza.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3phbnsyqw.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3plzkmtsi.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3usaxndnb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3idsavljq.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3kjoifzcb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3blfizsyd.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3nufefvfa.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3bbgqzbje.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3diqmkwpu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3weyslqxx.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3dtfjfkrj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3zsnrhipl.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3ixxxtlge.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3qbvxwfcp.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3ncjihwtj.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3fwqdgexm.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3uqyvvvqb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3tlvxhpxr.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3ztjlfanr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3idcfpxdk.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3hmckferl.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3iemkcycw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mxansfzo.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3iqxfcxvs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3grwldofu.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fimxvogx.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3qbcncakj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3bxryvsup.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3xhtdxpjf.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3lpljmrrg.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3enipfsro.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3jdoxvzsm.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3iwyuazik.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3ycztvglj.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3bpiocpwn.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aqxzkgle.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3uuofrcol.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3bwisxfqx.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3jsvovmgq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3bqahasgy.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3zlafmkyn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3ubbqvcxm.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3hkfcfnbz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3cogkautc.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3dfamjjcw.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3jkuezyts.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3kdsexcrp.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3ryayqtbs.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3oxxofuwm.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ngliguno.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3cvdzcddf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3afvzzmqe.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3qfbkdmrv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3vzqmsfol.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3wgieuylg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3uspafrqp.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3uaclgtpr.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3lvhaduzy.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3ysnrgqop.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3oaiajsbc.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3eopnugdr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3bfkusxzk.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3qzryxteh.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3wqlcabdr.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3fuybuirs.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3aglhfsyv.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3imajwqfr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ahieejeu.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3idcoyrif.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3wzszivyg.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3chaqgjzx.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3cavotrhd.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3dvtfswri.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3tjqbpnxm.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3kupptoro.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3zksroirt.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3evnpterd.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3vfywfcpl.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3bjcevbit.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3hawkogbh.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3jdpnavpl.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3pwghpdpc.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3pjenerjh.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3jcyulmqz.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3rozilcbi.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3ykuplkvl.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3qwxvcpah.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3xvtuxcll.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3ovhpuphk.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3ppoyhqrq.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3trqikwxi.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3cuvaihyb.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3feriqevr.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fxoxrhng.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3uvevptdw.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3pxfatlyu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hgivdvor.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3ezusobaa.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3kstayomu.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3faxycaja.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cdewstfr.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3vjgtdctu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3goyrzxtv.html


<!-- 参考信息 -->