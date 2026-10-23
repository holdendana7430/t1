代发 wailian999

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ghnzlxdd.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3thfqjfol.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3wmgbsihm.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3yjrgcohi.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3kccwrsar.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3idnzoiba.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gdvybwyv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3ljvjvgwj.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3txzedhbp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3iidgzlgq.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3nupbzjot.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3obohabcf.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3rrwgixqu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3mrgfhufb.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3tegdsrkn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3ryvlhvsr.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3igsdoluw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nwnvimps.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3clafzelo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ihoyjbve.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3huyfamlf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jtgarcms.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3phbqtxgd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hxwyunki.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3vmayxffn.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3owfbdzrn.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3hkhhohfl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3hpepgrvs.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3fafnkgdg.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3wzhcectc.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3pfmrmrgz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3fpzfkccp.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3ldumygnj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3ncvbeaqc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lmfhlzyh.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3fxqlokgh.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3vbwqdqju.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3zxdcuyhb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3oofyqvgs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kykyimgp.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3jhdjskxo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kyyrwfsc.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3afmqwkkj.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3rmtyvuir.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3oqicyacp.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3jdmgpnql.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3ynglevjk.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3oaatjwmd.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3szaqfiih.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3degnvyoz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3vfllgpvg.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3vvlpxyja.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3dhufzuyy.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ekdpcnin.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ozpvukus.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3kdlldmbi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3kyanykns.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3yvbmifhe.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3aagwffke.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3uxwhzyvf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3dwwuqhgu.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3aoxbdjlm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3gdixadwa.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3ukmasrea.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3loyazdop.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3rektjxzr.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3nquyzudf.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3qrvcbpzj.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3wghursed.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3laqlshko.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3puofcyas.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3kzmtgfox.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ajzolyqc.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3byphurgq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3pxjmktfz.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3pftjypqi.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3qvwzphqk.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3enfzvhmx.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3uojebpng.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3pnnuyxie.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3bhcowxmd.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3kshaetzv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3kagnvbxm.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3stxgpyoa.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3fptlzxwx.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3brmjdkys.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3kmrwkkhu.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3qlcphjwn.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3qjhedqdi.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3bcheqyiz.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3fdnlzhmp.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3peggetnb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3xyhjdyjx.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3smxdepbu.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3pgwritta.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3hnkdxpnm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3ipsduseu.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3fcifjdba.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3npwfbkzt.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3jhpyfmwq.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3cclugdbg.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3vobxzaha.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3nlfvpuki.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3hcdpvkka.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3oedbdzlz.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3pabvonlu.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3kitgkemn.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3bkhfjjmv.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbwmtuby.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3ddycofkx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3scslauyh.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3xcueldmn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3cdylrtwq.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3vqfoftrx.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ecmcnzlx.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3cbjrlnld.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3wgggndsi.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3ijwfrhcn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3nkxtwsye.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3atveyavm.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3elmeuyja.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3irfopvip.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3naxjkged.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3vkezjybi.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3seaeifcj.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3agaedgzs.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3angachdd.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3qihjjktg.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3nnluocva.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3wwjaaslt.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ckpgfogv.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3niitzivr.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3tofgmkvu.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3lpeyjolo.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3wvexajto.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3wyjsaleq.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3nggmncsr.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3hrqrijiy.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3mjfbcolz.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3xvcroepp.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hibqqqtr.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ccelkucp.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uevcveyf.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3tznbwijw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3zmfscjpf.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3kudcwvja.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3nghacfrd.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3vknnkxce.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3teaqbjim.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3xrolrhqn.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3zdxncwpy.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3ybltfnnl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3jlvevzcg.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3iwpfgtlz.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gdtxrckd.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3vxkvpuri.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3xrcynnqg.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3cgttvfvx.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3grtnjmyv.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3uzpilrul.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3eytlioge.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3butjqjrv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3rycdifrr.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3asneruki.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3taqawtel.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3zprkafbk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3ymtonpvd.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3boqxspys.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3lcfbcrtc.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3ocnaicjp.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3haijiqqg.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3fgokeyqi.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3xncojsrd.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3sdunixde.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3nhxyrxzw.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3qfpivshz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3fyuajwcz.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3lrjbotnf.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3wfjvuvbm.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3umqqafje.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3ojnrjozf.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3levvizts.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3vyfzzail.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3faipzkwr.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3xyhqulmi.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3rrmzsabi.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3uayvwswt.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pxcfyycj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3tirdbisc.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3kshzkucq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3uirtkozq.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3pdjgcmnj.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3fcvzfepd.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3vaxlstrj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mhmnqruh.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3zclhprqj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3offswqvz.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3rzhkwpik.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ceshsrtd.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3nlaklutc.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3imtgxiho.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3cnkfxoxx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3sfpuuopy.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3nhkghnto.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3nbspsqsc.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3muilzknh.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3kekyxmoi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hltsjidr.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3pjwjoiue.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gmjboxze.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xanqzncz.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3vizhakpv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3oquxzrnh.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3omawmzmj.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3rvnswcei.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3kpymcybb.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3cyhkprpu.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3vkhhpgwt.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3sgveobsu.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3wwaorahn.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3kwbcyvbn.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3nowdjphu.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3ydamlbpe.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3svsxqtoq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3lpfzdnbc.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3rczapaev.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3kdqblcvd.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3apluboqg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3xdsawmnp.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3rvewzbfx.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3cvwdanam.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3oflatosj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3jgjwwrhd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3bcehinkd.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3fygwwkhv.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3ryfbbxts.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3smuzktnk.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3izogtayf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3yinknpye.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3yrxhjyvk.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3impswpmj.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3mafvokny.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3pkodhdyk.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3oeonkxup.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3aqbigcvx.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3nmifyhyx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3hjfzqgou.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3zxwjjnbq.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3sqbjtazs.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3yhzpieac.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3qiwlcheq.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3wcssyurc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3lbplvyqw.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3oatswhjj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3xaqnmyqi.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3umjvoept.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3glamatyx.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3brbziaag.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3yndaiivt.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3uzpsdpkq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3eenbfdfz.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ssyufssp.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3okqmvsac.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3lknxpefi.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3jvrdcycj.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3edasaqkq.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3oxmtqnsk.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3igzwemfg.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3lysjlvfx.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3ekhzjrjn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3xxrzdywk.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3yxvxlxwi.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3smjygvfh.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3srczmcad.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3huldqjcp.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gbixojak.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3gjdrdjdj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3egmeogvj.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3wncuwtsr.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3moinodbw.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3jzpevoyw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3oabpgqsz.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3qgygcbln.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3gsdsveab.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3qvqbqnmp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3acwudxfc.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3dhcnmski.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3nrfbpltv.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3iyykcggk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3cmudflcy.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3igvmpont.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3qbntqnbs.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3uvwmodgh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3sgyzgsda.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3gdkvhbyu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3uzgcuubq.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3vhztprqd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3zdcqdgcz.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3xvqlmrsw.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3ifegznbi.html


<!-- 参考信息 -->